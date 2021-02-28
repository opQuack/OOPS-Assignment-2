```java

import java.io.*;

public class question9 extends Exception {
    private static final long serialVersionUID = 1L;

    public static void validate(File f, int k) {
        long a = f.length();
        System.out.println(a);
        if(a <= k)
            throw new ArithmeticException("Lower than " + k);
    }
    public static void main(String[] args){
        File f = new File("demo.txt");
        validate(f, 2500);
    }
}


```
