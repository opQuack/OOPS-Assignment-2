```java
class parent{
    public void identify(){
        System.out.println("This is parent class.");
    }
}

class child extends parent{
    public void identify(){
        System.out.println("This is child class.");
    }
    public void parentIdentify(){
        super.identify();
    }
}

public class question1{
    public static void main(String[] args){
        parent P = new parent();
        child C = new child();

        System.out.println("\nCalling from Parent: ");
        P.identify();
        System.out.println("\nCalling from Child: ");
        C.identify();
        C.parentIdentify();
    }
}
```
