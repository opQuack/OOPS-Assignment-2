```java
class Shape{
    public void identify(){
        System.out.println("This is a shape");
    }
}

class Rectangle extends Shape{
    public void identify(){
        System.out.println("This is a rectangle shape");
    }
    protected void parentIdentify(){
        super.identify();
    }
}

class Circle{
    public void identify(){
        System.out.println("This is a Circle shape");
    }
}

class Square1 extends Rectangle{
    public void identify(){
        System.out.println("Square is a rectangle");
    }
    public void parentIdentify(){
        super.identify();
        super.parentIdentify();
    }
}

public class question6 {
    public static void main(String[] args){
        Square1 s = new Square1();
        s.identify();
        s.parentIdentify();
    }
}


```
