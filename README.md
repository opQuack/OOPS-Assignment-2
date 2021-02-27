```java
import java.util.Scanner;

class Rectangle{
    private double length_;
    private double breadth_;
    Rectangle(double l, double b){
        length_ = l;
        breadth_ = b;
    }
    public double Area(){
        return length_ * breadth_;
    }
    public double Perimeter(){
        return 2 * ( length_ + breadth_ );
    }
    public void displayStats(){
        System.out.println("Area: " + Area());
        System.out.println("Perimeter: " + Perimeter() + "\n");
    }
}

class Square extends Rectangle{
    public Square(double s){
        super(s, s);
    }
    public void displayStats(){
        super.displayStats();
    }
}

public class question4 {
    public static void main(String[] args){
        double i, j;
        Scanner sc = new Scanner(System.in);
        i = sc.nextDouble();
        j = sc.nextDouble();
        
        Rectangle R = new Rectangle(i, j);
        System.out.println("\nRectangle:");
        R.displayStats();

        i = sc.nextDouble();
        Square S = new Square(i);
        System.out.println("\nSquare:");
        S.displayStats();
    }
}

```
