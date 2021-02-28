```java

class student{
    static int cnt;
    String name;
    student(String n){
        if(cnt == 5)
            throw new ArithmeticException("Not more than 5 can be created");
        cnt++;
        name = n;
    }
}

public class question10 {
    public static void main(String[] args){
        int i;
        student s;
        for( i = 0; i < 6; i++ ){
            try{
                s = new student("Vivaldi");
                System.out.println(i);
                s = null;
            }
            catch(ArithmeticException e){
                System.out.println(e.getMessage());
            }
            
        }

    }
}



```
