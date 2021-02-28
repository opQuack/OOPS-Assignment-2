```java


class allAdds{
    public int add(int a, int b){
        return a+b;
    }
    public int add(int a, int b, int c){
        return a+b+c;
    }
}

public class question7 {
    public static void main(String[] args){
        allAdds A = new allAdds();
        System.out.println(A.add(2, 3));
        System.out.println(A.add(2, 3, 4));
    }
}



```
