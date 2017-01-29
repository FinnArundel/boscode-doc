# Software Design & Development - Learning activities

See also [boscode-learn](https://github.com/Quobject/boscode-learn#table-of-content)

## Table of content

[1 Object oriented paradigm](#1-object-oriented-paradigm)

[1.1 Shape class](#11-shape-class)  
[1.2 Getters and setters](#12-getters-and-setters)  
[1.3 Shape class with print method](#13-shape-class-with-print-method)  
[1.4 Circle class](#14-circle-class)   
[1.5 Composition - Car cost](#15-composition---car-cost)    
[1.6 Constructor - Plant](#16-constructor---plant)  


___
## 1 Object oriented paradigm

### 1.1 Shape class

* Pseudocode

```
class Shape {
  private -
    shape_no: integer
    x_coordinate: double
    y_coordinate: double
  public -
    getXCoordinate():
      return x_coordinate
    
    setXCoordinate(value):
      x_coordinate = value
}

BEGIN Main
  shape = new Shape()
  shape.setXCoordinate(23)

  Display shape.getXCoordinate()

END Main

```

* C#

```cs
using System;

namespace yr12sdd
{

    public class Shape
    {
        private int shape_no;
        private double x_coordinate;
        private double y_coordinate;

        public double getXCoordinate()
        {
            return x_coordinate;
        }

        public void setXCoordinate(double value)
        {
            this.x_coordinate = value;
        }

    }


    class Program
    {
        static void Main(string[] args)
        {
            Shape shape = new Shape();

            shape.setXCoordinate(23);
            Console.WriteLine(shape.getXCoordinate());

            Console.ReadLine();

        }
    }

}

```

1. Run the above C# code on your laptop
2. Modify the code to:
  * create another instance of a shape object with the variable name of `shape2`
  * set the X coordinate of the new shape to 50
  * print out the X coordinate of this new Shape
3. Run and test your program
4. Write a pseudocode version of your modified C# code.
5. Paste C# and pseudocode into you solution google drive document.

___



### 1.2 Getters and setters

* Pseudocode

```
class Shape {
  private -
    shape_no: integer
    x_coordinate: double
    y_coordinate: double
  public -
    getXCoordinate():
      return x_coordinate
    
    setXCoordinate(value):
      x_coordinate = value
}

BEGIN Main
  shape = new Shape()
  shape.setXCoordinate(23)

  Display shape.getXCoordinate()

END Main

```

The above pseudocode has the private attribute `x_coordinate`. To be able to change the value of this attribute outside of an object of a `Shape` data type there are two public methods: `getXCoordinate` and `setXCoordinate`. These two methods are called getter and setter methods.

* Modify the above pseudocode to implement a getter and setter for the other two private attributes `shape_no` and `y_coordinate`.  
* Modify the Main function to set the `shape_no` to `1` and the `y_coordinate` to `42`.  
* Modify the Main function to produce the following output using the shape object:  
```
Shape Number: 1
X coordinate: 23
Y coordinate: 42
```
* Write a C# version of your modified pseudocode.

___

### 1.3 Shape class with print method


* C#

```cs
using System;

namespace yr12sdd
{

    public class Shape
    {
        private int shape_no;
        private double x_coordinate;
        private double y_coordinate;

        public double getXCoordinate()
        {
            return x_coordinate;
        }

        public void setXCoordinate(double value)
        {
            this.x_coordinate = value;
        }

    }


    class Program
    {
        static void Main(string[] args)
        {
            Shape shape = new Shape();

            shape.setXCoordinate(25);
            Console.WriteLine(shape.getXCoordinate());

            Console.ReadLine();

        }
    }

}

```

The above C# code instantiates a Shape object, sets the x_coordinate to 25 and outputs the value of the x_coordinate to the console.  
* Run the above code.  
* Add a new method to the Shape class called `print()`. This method does not return a value and also does not take any arguments. Calling this method should produce the following console output (using the current value of the x_coordinate attribute):

```
X coordinate: 23
```

* Run and test your program
* Write a pseudocode version of your modified C# code.

___


### 1.4 Circle class

* Pseudocode

```
class Shape {
  private -
    shape_no: integer
    x_coordinate: double
    y_coordinate: double
  public -
    getShapeNo():
      return shape_no

    setShapeNo(value):
      shape_no = value

    getXCoordinate():
      return x_coordinate

    setXCoordinate(value):
      x_coordinate = value

    getYCoordinate():
      return y_coordinate

    setYCoordinate(value):
      y_coordinate = value

    getArea():
      return 0.0

    print():
      Display "*** Shape ***"
      Display "Shape Number: ", getShapeNo()
      Display "X coordinate: ", getXCoordinate()
      Display "Y coordinate: ", getYCoordinate()
      Display "Area: ", getArea()
}

sub-class Circle {
  is a Shape
  private -
    radius: double
  public -
    getRadius():
      return radius

    setRadius(value):
      radius = value

    getArea():
      return radius * radius * Math.PI    

    print():
      Display "*** Circle ***"
      Display "Shape Number: ", getShapeNo()
      Display "X coordinate: ", getXCoordinate()
      Display "Y coordinate: ", getYCoordinate()
      Display "Radius: ", getRadius()    
      Display "Area: ", getArea()    
}

BEGIN Main
  shape = new Shape()
  shape.setShapeNo(1)
  shape.setXCoordinate(25)
  shape.setYCoordinate(42)

  circle = new Circle()
  circle.setShapeNo(2)
  circle.setRadius(35)
  circle.setXCoordinate(267)
  circle.setYCoordinate(190)

  shapeArray(1) = shape
  shapeArray(2) = circle

  FOR i = 1 TO 2 STEP 1
    shapeArray(i).print()
  NEXT i



END Main

```

* C#

```cs
using System;

namespace yr12sdd
{

    public class Shape
    {
        private int shape_no;
        private double x_coordinate;
        private double y_coordinate;

        public int getShapeNo()
        {
            return shape_no;
        }

        public void setShapeNo(int value)
        {
            this.shape_no = value;
        }

        public double getXCoordinate()
        {
            return x_coordinate;
        }

        public void setXCoordinate(double value)
        {
            this.x_coordinate = value;
        }

        public double getYCoordinate()
        {
            return y_coordinate;
        }

        public void setYCoordinate(double value)
        {
            this.y_coordinate = value;
        }

        public virtual double getArea()
        {
            return 0.0;
        }

        public virtual void print()
        {
            Console.WriteLine("*** Shape ***");
            Console.WriteLine("Shape Number: " + this.getShapeNo());
            Console.WriteLine("X coordinate: " + this.getXCoordinate());
            Console.WriteLine("Y coordinate: " + this.getYCoordinate());
            Console.WriteLine("Area: " + this.getArea());
        }

    }


    public class Circle : Shape
    {
        private double radius;

        public double getRadius()
        {
            return radius;
        }

        public void setRadius(double value)
        {
            this.radius = value;
        }

        public override double getArea()
        {
            return radius * radius * Math.PI;
        }

        public override void print()
        {
            Console.WriteLine("*** Circle ***");
            Console.WriteLine("Shape Number: " + this.getShapeNo());
            Console.WriteLine("X coordinate: " + this.getXCoordinate());
            Console.WriteLine("Y coordinate: " + this.getYCoordinate());
            Console.WriteLine("Radius: " + this.getRadius());
            Console.WriteLine("Area: " + this.getArea());
        }

    }


    class Program
    {
        static void Main(string[] args)
        {
            Shape shape = new Shape();
            shape.setShapeNo(1);
            shape.setXCoordinate(25);
            shape.setYCoordinate(42);

            Circle circle = new Circle();
            circle.setShapeNo(2);
            circle.setRadius(35);
            circle.setXCoordinate(267);
            circle.setYCoordinate(190);

            Shape[] shapeArray = new Shape[2];
            shapeArray[0] = shape;
            shapeArray[1] = circle;

            for( int i = 0; i< shapeArray.Length; i++)
            {
                shapeArray[i].print();
            }

            Console.ReadLine();

        }
    }

}

```

1. Run the above C# code on your laptop.
2. Modify the pseudocde and C# code to include a rectangle shape class.
3. Modify the pseudocde and C# code: The Main function should create 3 circles and 2 rectangles before printing all 5 shapes details to the console using a counted loop and producing exactly the following output:
```
*** Circle ***
Shape Number: 1
X coordinate: 267
Y coordinate: 190
Radius: 35
Area: 3848.4510006475
*** Circle ***
Shape Number: 2
X coordinate: 90
Y coordinate: 55
Radius: 46
Area: 6647.610054996
*** Circle ***
Shape Number: 3
X coordinate: -34
Y coordinate: 85
Radius: 6
Area: 113.097335529233
*** Rectangle ***
Shape Number: 4
X coordinate: 68
Y coordinate: 78
Height: 20
Width: 8
Area: 160
*** Rectangle ***
Shape Number: 5
X coordinate: 998
Y coordinate: 783
Height: 20
Width: 8
Area: 160
```

___


### 1.5 Composition - Car cost

From question 33 (d) [BOS 2015-hsc-sdd](http://www.boardofstudies.nsw.edu.au/hsc_exams/2015/exams/2015-hsc-sdd.pdf). A custom car manufacturer makes cars to order based on customers’ selections of components. Each component may be standard or specialised.  
The cost of a car is calculated by totalling the costs of all components. The cost of each standard component is fixed. The cost of a specialised component is calculated by adding the cost of the specialisation to the cost of the standard component.  
The software to manage customers’ selections is being developed. This fragment of code has been designed to be part of the software.  

A standard engine costs $2000, but a V8 engine costs an extra $800.  

* Pseudocode

```
class Car {
  private –
    components: array of Component
  public –
    getComponents():
      return components

    setComponents(value):
      components = value

    cost():
      sum = 0
      FOR i = 1 TO number of components
        sum = sum + components[i].cost()
      NEXT i
      return sum
}
class Component {
  public –
    cost(): REM returns the cost of the component
}
class Engine {
  is a Component
}
class V8Engine { 
  is a Engine 
}

BEGIN Main
  car = new Car()

  componentsForCar(1) = new Engine()
  car.setComponents(componentsForCar)

  Display car.cost()

END Main

```

1. Write the cost() method to calculate the cost of instances of the Engine and V8Engine subclasses of Component.  
2. Write another subclass of Component `Wheel` with a cost of $200, and inside the Main function add 4 instances of this class to the car  
3. Inside Main create an additional Car instance with a V8Engine and 6 wheels and display the total cost.
4. Write a C# implementation of your solution.    

___  

### 1.6 Constructor - Plant

From question 33 (d) [BOS 2016-hsc-sdd](http://www.boardofstudies.nsw.edu.au/hsc_exams/2016/exams/2016-hsc-sdd.pdf). 
The following fragment of code was developed using the object oriented paradigm (OOP).

* Pseudocode

```
class Plant {
  private –
    id: integer
  public –
    Plant()

    Plant(idParameter)
	  id = idParameter
    END Plant(idParameter)

	Name: string
	Description: string
	Colour: string
	getID()
      RETURN id
	END getID
}

class Fruit {
  is a Plant

  public –
    Fruit()
	NumberOfSeeds: integer
	isSweet: boolean
}

class Vegetable {
  is a Plant

  public –
    Vegetable()
	GrowsAboveGround: boolean
}


BEGIN Main
  carrot = new Vegetable()

  carrot.Name = "Carrot"
  carrot.Description = "root vegetable"
  carrot.Colour = "orange"
  carrot.GrowsAboveGround = false

  Display carrot.Name
END Main

```

* C#

[dotnedfiddle](https://dotnetfiddle.net/CShYFI)

```cs
using System;
	

public class Plant{
	private int id;
	
	public Plant(){
	}	
	
	public Plant(int idParameter){
		this.id = idParameter;
	}
	
	public string Name;
	public string Colour;
	public string Description;
	
	public int getID(){
		return this.id;
	}
}

public class Fruit : Plant{
	
	public Fruit(){
	}
	
	public int NumberOfSeeds;
	public bool IsSweet;
}


public class Vegetable : Plant{
	
	public Vegetable(){
	}
	
	public bool GrowsAboveGround;
}


public class Program
{
	public static void Main()
	{
		Vegetable carrot = new Vegetable();		
		carrot.Name = "Carrot";
		carrot.Colour = "orange";
		carrot.Description = "root vegetable";
		carrot.GrowsAboveGround = false;
		
		Console.WriteLine(carrot.Name);
		
	}
}

```
