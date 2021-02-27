```java
import java.util.Scanner;

class Member{
    private String name_;
    private int age_;
    private String phone_number_;
    private String address_;
    private double salary_;
    Member(){
        name_ = phone_number_ = address_ = "";
        age_ = 0;   
    }
    public void set(){
        Scanner sc = new Scanner(System.in);
        name_  = sc.next();
        age_ = sc.nextInt();
        phone_number_ = sc.next();
        address_ = sc.next();
        salary_ = sc.nextDouble();
    }
    protected void printSalary(){
        System.out.println("Salary: " + salary_);
    }
    protected void print(){
        System.out.println("Name: " + name_);
        System.out.println("Age: " + age_);
        System.out.println("Phone Number: " + phone_number_);
        System.out.println("Address: " + address_);
        printSalary();
    }
}

class Employee extends Member{
    private String specialization_;
    Employee(){
        specialization_ = "";
    }
    public void set(){
        Scanner sc = new Scanner(System.in);
        super.set();
        specialization_ = sc.next();
    }
    public void print(){
        super.print();
        System.out.println("Specialization: " + specialization_ + "\n");
    }

}

class Manager extends Member{
    private String dept_;
    Manager(){
        dept_ = "";
    }
    public void set(){
        Scanner sc = new Scanner(System.in);
        super.set();
        dept_ = sc.next();
    }
    public void print(){
        super.print();
        System.out.println("Department: " + dept_ + "\n");
    }
}

public class question3 {
    public static void main(String[] args){
        Employee E = new Employee();
        Manager M = new Manager();
        System.out.println("\nEmployee: ");
        E.set();
        System.out.println("\nManager: ");
        M.set();
        System.out.println("\n");
        E.print();
        M.print();
    }
}

```
