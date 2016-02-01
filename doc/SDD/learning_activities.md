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





### 1.5 

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









