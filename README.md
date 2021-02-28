```java

class numPair{
    int a;
    int b;
    public void display(){
        System.out.print(a + " " + b);
    }
}

public class question12 {
    public static void main(String[] args){
        numPair a = new numPair();
        String b;
        int[] d;
        //1
        try{
            a = null;
            a.display();
        }
        catch(NullPointerException e){
            System.out.println(e.getMessage());
        }
        //2
        try{
            throw null;
        }
        catch(NullPointerException e){
            System.out.println(e.getMessage());
        }
        //3
        try{
            b = null;
            int c = b.length();
        }
        catch(NullPointerException e){
            System.out.println(e.getMessage());
        }
        //4
        try{
            d = null;
            System.out.print(d[1]);
        }
        catch(NullPointerException e){
            System.out.println(e.getMessage());
        }
    }

}


```
