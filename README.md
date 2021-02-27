```java
class parent1{
    private void identify(){
        System.out.println("This is parent class.");
    }
}

class child1 extends parent1{
    public void identify(){
        System.out.println("This is child class.");
    }
    public void parentIdentify(){
            super.identify();
    }
}

public class question2{
    public static void main(String[] args){
        parent1 P = new parent1();
        child1 C = new child1();
        System.out.println("\nCalling from Parent: ");
        P.identify();
        System.out.println("\nCalling from Child: ");
        C.identify();
        C.parentIdentify();
    }
}
```
