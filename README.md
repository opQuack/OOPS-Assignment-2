```java
import java.util.Scanner;
import java.util.Vector;

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

public class question5 {
    public static void main(String[] args){
        int i, n;
        double j;
        Scanner sc = new Scanner(System.in);
        
        System.out.print("n: ");
        n = sc.nextInt();
        Vector<Square> s = new Vector<Square>();
        for( i = 0; i < n; i++ ){
            j = sc.nextDouble();
            s.add(new Square(j));
            System.out.println("Square " + (i+1) + ": ");
            s.elementAt(i).displayStats();
        }

        
    }
}

```
