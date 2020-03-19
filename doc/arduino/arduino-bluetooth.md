
# Arduino Bluetooth

[Arduino Compatible Bluetooth® V4.0 BLE Module](https://www.jaycar.com.au/arduino-compatible-bluetooth-v4-0-ble-module/p/XC4382)

### bluetooth.ino

```c
#include <SoftwareSerial.h>

int state = 0;
int count = 0;
SoftwareSerial mySerial(2,3);
char str[80];
long randNumber;

 
void setup() {
 mySerial.begin(9600);                 
 Serial.begin(9600); // Default connection rate for my BT module
 randomSeed(analogRead(0));
}
 
void loop() {

  if (mySerial.available()) {
    state = mySerial.read();
    Serial.write(state);
  }

  if (count++ > 100) {
     randNumber = random(300);
     sprintf(str, "s = %d\0", randNumber);
     mySerial.write(str); 
     count = 0;
  }

  delay(10);
}
```

### ViewController.swift

```swift
import CoreBluetooth
import UIKit

class ViewController: UIViewController, CBPeripheralDelegate, CBCentralManagerDelegate {
    public static let SERVICE_NAME = "HMSoft"
    private let SCAN_NUMBER_OF_ITEMS = 10;
    private var scans = 0;
    
    private var centralManager: CBCentralManager!
    private var peripheralDict: [String: CBPeripheral] = [:];
    private var peripheral: CBPeripheral!
    private var characteristic: CBCharacteristic!
    
    @IBOutlet weak var scanButton: UIButton!
    
    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view.
        centralManager = CBCentralManager(delegate: self, queue: nil)
        scanButton.isEnabled = false
    }
    
    func centralManagerDidUpdateState(_ central: CBCentralManager) {
        print("Central state update")
        if central.state != .poweredOn {
            print("Central is not powered on")
        } else {
            scanButton.isEnabled = true
        }
    }
    
    @IBAction func writeButton(_ sender: Any) {
        if self.characteristic != nil {
            self.write("Hello world")
        }
    }
 
    
    @IBAction func scan(_ sender: Any) {
        print("Central scanning");
        centralManager.scanForPeripherals(withServices: [], options: [CBCentralManagerScanOptionAllowDuplicatesKey : true])
        
    }
    
    
    func centralManager(_ central: CBCentralManager, didDiscover peripheral: CBPeripheral, advertisementData: [String : Any], rssi RSSI: NSNumber) {
        if (scans > SCAN_NUMBER_OF_ITEMS) {
            self.centralManager.stopScan()
            print("scanning done");
            for (_, _) in peripheralDict {
                //print("did discover \(name)")
            }
            if let p = peripheralDict[ViewController.SERVICE_NAME] {
                print("found: \(ViewController.SERVICE_NAME)");
                self.peripheral = p;
                self.peripheral.delegate = self
                self.centralManager.connect(self.peripheral, options: nil)
            } else {
                print("not found: \(ViewController.SERVICE_NAME)");
            }
        }
        scans += 1;
        
        if let name = peripheral.name {
            //let uid = peripheral.identifier
            
            if peripheralDict[name] == nil {
                peripheralDict[name] = peripheral;
            }
        }
        
        // Connect!"
        //self.centralManager.connect(self.peripheral, options: nil)
    }
    
    // The handler if we do connect succesfully
    func centralManager(_ central: CBCentralManager, didConnect peripheral:
        CBPeripheral) {
        if peripheral == self.peripheral {
            print("Connected to your \(ViewController.SERVICE_NAME) Board")
            peripheral.discoverServices(nil)
        }
        
    }
    
    
    func peripheral(_ peripheral: CBPeripheral, didDiscoverServices error: Error?) {
        //print("didDiscoverServices")
        if let services = peripheral.services {
            for service in services {
                //print("service found \(service.uuid)")
                peripheral.discoverCharacteristics([], for: service);
                //return;
            }
        }
    }
    
    func peripheral(_ peripheral: CBPeripheral, didDiscoverCharacteristicsFor service: CBService, error: Error?) {
        if let e = error {
            print("ERROR didDiscoverCharacteristicsFor \(e)")
            return
        }
        if let characteristics = service.characteristics {
            //print("didDiscoverCharacteristicsFor \(service.uuid)")
            //            for characteristic in characteristics {
            //                print("characteristics \(characteristic.uuid)")
            //            }
            self.characteristic = characteristics[0];
            //printCharacteristicProperties();
            peripheral.readValue(for: characteristic)
            peripheral.setNotifyValue(true, for: self.characteristic)
            
        }
    }
    
    func peripheral(_ peripheral: CBPeripheral, didUpdateValueFor characteristic: CBCharacteristic, error: Error?) {
        
        //print("didUpdateValueFor \(characteristic)")
        guard let data = characteristic.value else { return }
        //print("didUpdateValueFor \(data)")
        
        if let ds = String(data: data, encoding: String.Encoding.utf8) {
            print("didUpdateValueFor message = '\(ds)'")
        }
        
        
    }
    
    func write(_ value: String) {
        
        let value1 = value.data(using: String.Encoding.utf8)
        
        if let v = value1 {
            if let ch = self.characteristic {
                self.peripheral.writeValue(v, for: ch, type: .withoutResponse);
                print("write \(value) ");
            }
            
        }
    }
    
    func printCharacteristicProperties() {
        if let char = self.characteristic {
            if char.properties.contains(.writeWithoutResponse) {
                print("char.properties.contains(.writeWithoutResponse)")
            }
            
            if char.properties.contains(.read) {
                print("char.properties.contains(.read)")
            }
            
            print("property found: \(char.properties)")
        }
    }
}
```