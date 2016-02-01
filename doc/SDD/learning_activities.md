# Software Design & Development - Learning activities

## Table of content


___
## 1 Object oriented paradigm

### 1 Point class

* Pseudocode

```
class Point {
  private -
    point_no: integer
    x_coordinate: double
    y_coordinate: double
  public -
    getXCoordinate():
      return x_coordinate
    
    setXCoordinate(value):
      x_coordinate = value
}

BEGIN Main
  point = new Point()
  point.setXCoordinate(23)

  Display point.getXCoordinate()

END Main

```

* C#

```cs
using System;

namespace ConsoleApplication1
{

    public class Point
    {
        private int point_no;
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
            Point point = new Point();

            point.setXCoordinate(25);
            Console.WriteLine(point.getXCoordinate());

            Console.ReadLine();

        }
    }

}

```




___
