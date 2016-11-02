# Software Design & Development - Learning activities

See also [boscode-learn](https://github.com/Quobject/boscode-learn#table-of-content)

## Table of content

1 Object oriented paradigm

[1.1 Installation](#11-installation)  
[1.2 Shape class](#12-shape-class)  
[1.3 Getters and setters](#13-getters-and-setters)  
[1.4 Shape class with print method](#14-shape-class-with-print-method)  
[1.5 Circle class](#15-circle-class)  
[1.6 Car cost](#16-car-cost) 
[1.7 Plant](#17-plant)  

2 Desk check

[2.1 Desk check 1](#21-desk-check-1)  
[2.2 Desk check 2](#22-desk-check-2)  
[2.3 Desk check 3](#23-desk-check-3)  
[2.4 Desk check 4](#24-desk-check-4)  
[2.5 Desk check 5](#25-desk-check-5)  
[2.6 Desk check 6](#26-desk-check-6)  
[2.7 Desk check 7](#27-desk-check-7)  
[2.8 Desk check 8](#28-desk-check-8)  
[2.9 Desk check 9](#29-desk-check-9)  
[2.10 Desk check 10](#210-desk-check-10)  
[2.11 Desk check 11](#211-desk-check-11)  
[2.12 Desk check 12](#212-desk-check-12)  
[2.13 Desk check 13](#213-desk-check-13)  
[2.14 Desk check 14](#214-desk-check-14)  
[2.15 Desk check 15](#215-desk-check-15)  
[2.16 Desk check 16](#216-desk-check-16)  
[2.17 Desk check 17](#217-desk-check-17)  
[2.18 Desk check 18](#218-desk-check-18)  
[2.19 Desk check 19](#219-desk-check-19)  
[2.20 Desk check 20](#220-desk-check-20)  
[2.21 Desk check 21](#221-desk-check-21)  
[2.22 Desk check 22](#222-desk-check-22)  
[2.23 Desk check 23](#223-desk-check-23)  
[2.24 Desk check 24](#224-desk-check-24)  
[2.25 Desk check 25](#225-desk-check-25)  
[2.26 Desk check 26](#226-desk-check-26)  



___
## 1 Object oriented paradigm

### 1.1 Installation

* Windows:
  1. Install [Visual Studio 2015 Community](https://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx)
  2. Start Visual Studio
  3. FILE > New > Project
    * Templates > Visual C# > Windows > Classic Desktop > Console Application
    * Name: yr12sdd

* Mac OS X:
  1. Install Xamarin 'Xamarin Starter Edition' https://xamarin.com/starter
  2. Start Xamarin Studio
  3. File > New > Solution
    * Other .NET
    * Console Project c#
    * Project Name: yr12sdd


### 1.2 Shape class

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



### 1.3 Getters and setters

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

### 1.4 Shape class with print method


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


### 1.5 Circle class

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


### 1.6 Car cost

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

### 1.7 Plant

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



___  
## 2 Desk check

### 2.1 Desk check 1

Consider this fragment of code

```
BEGIN
  length = 0
  breadth = 0
  area = length * breadth
  length = 5
  breadth = 4
END
```

1. Complete a desk check  
2. What are the values of length, breadth and area after the fragment of code has been executed?

___

### 2.2 Desk check 2

Consider this fragment of code

```
BEGIN
  m = 1
  p = 2
  m = p
  p = m
END
```

1. Complete a desk check  
2. What are the values of m and p after the fragment of code has been executed?

___

### 2.3 Desk check 3

Consider this fragment of code

```
BEGIN
  a = 2
  b = 4
  a = a + b
  b = a + b
  Display a, b
END
```

1. Complete a desk check  
2. What is the output from this fragment of code?

___

### 2.4 Desk check 4

Consider this algorithm

```
BEGIN
  x = 4
  y = x
  z = x * y
  Display z
END
```

1. Complete a desk check  
2. What is the output from this fragment of code?

___

### 2.5 Desk check 5

Consider this algorithm

```
BEGIN
  Get x
  WHILE x > 5
    Display x + 3
    x = x - 1
  ENDWHILE
END
```

1. Using the test data x = 7, complete a desk check.  
2. What is the output?


___



### 2.6 Desk check 6

Consider this algorithm

```
BEGIN
  n = 20
  CASEWHERE n is
    less than 10: n = n + 50
    less than 30: n = n + 10
    less than 50: n = n + 30
    OTHERWISE:    n = n + 50
  ENDCASE
  Display n
END
```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___



### 2.7 Desk check 7

Consider this algorithm

```
BEGIN
  number = 5
  WHILE number < 30
    Display number
    Increment number by 2
  ENDWHILE  
END
```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___



### 2.8 Desk check 8

Consider this algorithm

```
BEGIN
  number = -2
  REPEAT
    Display number
    number = number + 2
  UNTIL number > 10
END
```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___


### 2.9 Desk check 9

Consider this algorithm

```
BEGIN
  FOR number = 2 TO 10 STEP 1
    Display number * 2 + 1
  NEXT number
END
```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___


### 2.10 Desk check 10

Consider this algorithm

```
BEGIN
  number = 5
  REPEAT
    Display number
    Increment number by 2
  UNTIL number = 10  
END
```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___


### 2.11 Desk check 11

Consider this algorithm

```
BEGIN
  FOR number = 5 TO 13 STEP 2
    Display number
  NEXT number
END
```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___


### 2.12 Desk check 12

Consider this algorithm

```
BEGIN
  start = 4
  finish = 10
  WHILE start < finish
    start = finish - start
    finish = finish - 2
  ENDWHILE
END
```

1. Complete a desk check  
2. How many times will the statement within the body of the loop be executed?

___


### 2.13 Desk check 13

Consider this algorithm

```
BEGIN
  a = 1
  b = 2
  c = 3
  a = b
  c = a
  b = c
  Display a, b, c
END

```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___


### 2.14 Desk check 14

Consider this algorithm

```
BEGIN
  a = 10
  b = a - 2
  c = b / 2
  a = c + 5
  b = a - b
  Display b
END
```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___


### 2.15 Desk check 15

Consider this algorithm

```
BEGIN
  count = 10
  num = 10
  WHILE count > 0
    Display num - count
    count =  count - 2
  ENDWHILE
END
```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___




### 2.16 Desk check 16

Consider this algorithm

```
BEGIN
  count = 11
  num = 10
  WHILE count > 0
    count =  count - 2
    Display num - count
  ENDWHILE
END
```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___



### 2.17 Desk check 17

Consider this algorithm

```
BEGIN
  count = 10
  num = 10
  WHILE count > 0
    count =  count - 3
    Display num - count    
  ENDWHILE
END
```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___



### 2.18 Desk check 18

Consider this algorithm

```
BEGIN
  count = 10
  num = 10
  WHILE count > 0
    count =  count - 2
    Display num - count    
  ENDWHILE
END
```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___



### 2.19 Desk check 19

Consider this algorithm

```
BEGIN
  Get a
  Get b
  WHILE a < b
    Display a
    a = a + 3
  ENDWHILE 
END
```

1. Complete a desk check with the input 2 and 14. 
2. What is the output after the fragment of code has been executed with the input 2 and 14?

___




### 2.20 Desk check 20

Consider this algorithm

```
BEGIN
  Get a
  WHILE a > 0
    b = a * 2
    a = a - 1
    Display b
  ENDWHILE
END

```

1. Complete a desk check with the input 3. 
2. What is the output after the fragment of code has been executed with the input 3?

___



### 2.21 Desk check 21

a MOD b returns the remainder from the division a/b. For example, 11 MOD 4 = 3 because 11/4 = 2 remainder 3.

Consider this algorithm

```
BEGIN
  a = 15
  WHILE a > 1
    IF a MOD 2 = 0 THEN
      Display a
    ELSE
      a = a - 1
    ENDIF
  ENDWHILE
END
```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___



### 2.22 Desk check 22

Consider this algorithm

```
BEGIN
  x(1) = "a"
  x(2) = "b"
  x(3) = "c"
  x(4) = "d"
  x(5) = "e"

  i = 1
  j = number of elements in the array x
  WHILE i < j
    k = x(i)
    x(i) = x(j)
    x(j) = k
    i = i + 1
    j = j - 1
  ENDWHILE
END 
```

1. Complete a desk check  
2. Which of the following best describes what this code does?  
(A) It reverses the order of the elements in the array.  
(B) It copies the second half of th the array to the first half.  
(C) It copies the first half of the array to the second half.  
(D) It swaps the first half of the array and the second half of the array.  

___

### 2.23 Desk check 23

Consider this algorithm.

```
BEGIN order
  names(1) = "Smith" 
  names(2) = "Farelli" 
  names(3) = "Wu" 
  names(4) = "Andrews" 
  
  position = 1
  end = number of elements in the array names
  WHILE position < end
    current = position + 1
    maximum = position

    WHILE current <= end
      IF names(current) > names(maximum) THEN
        maximum = current
      ENDIF
      current = current + 1
    ENDWHILE
    `NOTE: the subprogram swap exchanges two elements of the array 'names'. 
    ` swap should be underlined
    swap(names, maximum, position)
    position = position + 1
  ENDWHILE
END order
```

1. Complete a desk check  

___



### 2.24 Desk check 24

Consider this algorithm

```
BEGIN main
  numA = 2
  numB = 3
  calc(numA, numB)
  Display numA, numB
END main

BEGIN calc(numC, numD)
  temp = numC
  WHILE numD > 1
    numC = numC * temp
    numD = numD - 1
  ENDWHILE
  Display numC, numD
END calc
```

1. Complete a desk check  
2. What is the output after the fragment of code has been executed?

___



### 2.25 Desk check 25

Consider this algorithm

```
BEGIN 
  list(1) = 1
  list(2) = 3
  list(3) = 5
  list(4) = 7
  list(5) = 9

  low = 1
  n = number of elements in the array list
  high = n
  WHILE low < n 
    list(low) = list(high)
    list(high) = list(low)
    low = low + 1
    high = high - 1
  ENDWHILE
END
```

1. Complete a desk check  


___







### 2.26 Desk check 26

Consider this algorithm

```
BEGIN
  a(1) = 1
  a(2) = 1
  i = 3
  WHILE i <= 10
    a(i) = a(i-1) + a(i-2)
    i = i + 1
  ENDWHILE
END
```

1. Complete a desk check  

___

