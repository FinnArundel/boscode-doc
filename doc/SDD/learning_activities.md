# Software Design & Development - Learning activities

## Table of content


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





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___





### 1.?

* Pseudocode

```


```

* C#

```cs


```

1. Run the above C# code on your laptop
2. Modify the code to:
  * 
3. Run and test your program
4. Write a pseudocode version of your modified C# code.

___









