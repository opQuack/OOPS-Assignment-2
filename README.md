```java

import java.util.*;

class StudentInfo{
    int id;
    String name;
    String dept_name;
    final String college_name = "NITW";
    
    public StudentInfo(int i, String n, String d) {
        id = i;
        name = n;
        dept_name = d;
    }

    public void display(){
        System.out.println("\nID: " + id + "\nName: " + name + "\nDept: " + dept_name + "\nCollege: " + college_name);
    }
}

public class StudentDatabase {
    public static void main(String[] args){
        HashMap<Integer, Boolean> Register = new HashMap<Integer, Boolean>();
        Vector<StudentInfo> S = new Vector<StudentInfo>();
        int t, i, id;
        String name, dept_name;
        Scanner sc = new Scanner(System.in);
        t = Integer.parseInt(sc.nextLine());
        for( i = 0; i < t; i++ ){
            id = Integer.parseInt(sc.nextLine());
            name = sc.nextLine();
            dept_name = sc.nextLine();
            try{
                if( Register.containsKey(id) == true )
                    throw new Exception("Duplicate Value");
                StudentInfo s = new StudentInfo(id, name, dept_name);
                S.addElement(s);
                Register.put(id, true);
            }catch(Exception e){System.out.println(e.getMessage());}
        }
        for( i = 0; i < t; i++ ){
            S.elementAt(i).display();
        }
        sc.close();
    }
}


```
