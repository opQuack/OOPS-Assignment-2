```java


package addPackage;

public class add {
    protected int a;
    protected int b;
    public add(int x, int y){
        a = x;
        b = y;
    }
    public int sumEm(){
        return a + b;
    }
}

package mulPackage;

public class multiply {
    protected int a;
    protected int b;
    public multiply(int x, int y){
        a = x;
        b = y;
    }
    public int mulEm(){
        return a * b;
    }       
}

package subPackage;

public class subtract {
    protected int a;
    protected int b;
    public subtract(int x, int y){
        a = x;
        b = y;
    }
    public int subEm(){
        return a - b;
    }    
}

import addPackage.*;
import mulPackage.*;
import subPackage.*;

class forDiv extends add{
    protected int num;
    forDiv(int x, int y){
        super(y, y);
        num = x;
    }
    public int division(){
        int res = 0, temp = 0;
        while(temp < num){
            temp = sumEm();
            res++;
        }
        return res;
    }
}

public class question8{
    public static void main(String[] args){
        add A = new add(2, 3);
        System.out.println(A.sumEm());
        subtract B = new subtract(3, 4);
        System.out.println(B.subEm());
        multiply C = new multiply(2, 3);
        System.out.println(C.mulEm());
        forDiv D = new forDiv(4, 1);
        System.out.println(D.division());
    }
}



```
