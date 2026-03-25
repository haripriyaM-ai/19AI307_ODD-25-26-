# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Write a Java program to demonstrate the concept of **class and object** by storing and displaying vehicle details.

---

## AIM:
To write a Java program to demonstrate the **class and object concept by creating objects and accessing their attributes**.

---

## ALGORITHM :
1. Start the program.  
2. Import the necessary package `java.util`.  
3. Create a class named `Main`.  
4. Define an inner class `Vehicle` with attributes `number`, `type`, and `owner`.  
5. Inside the `main()` method create a `Scanner` object.  
6. Create the first object `v1` of class `Vehicle`.  
7. Read vehicle number, type, and owner name for `v1`.  
8. Create the second object `v2` of class `Vehicle`.  
9. Read vehicle number, type, and owner name for `v2`.  
10. Display the details of both vehicles using the object variables.  
11. Stop the program.

---

## PROGRAM:

```java
/*
Program to implement a Class and Objects using Java
Developed by: HARI PRIYA M 
RegisterNumber: 212224240047  
*/

import java.util.Scanner;

public class Main {
    public static class Vehicle{
        String number;
        String type;
        String owner;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Vehicle v1 = new Vehicle();
        v1.number = sc.next();
        v1.type = sc.next();
        v1.owner = sc.next();

        Vehicle v2 = new Vehicle();
        v2.number = sc.next();
        v2.type = sc.next();
        v2.owner = sc.next();

        System.out.println(v1.number + " | " + v1.type + " | " + v1.owner);
        System.out.println(v2.number + " | " + v2.type + " | " + v2.owner);

        sc.close();
    }
}
```

---

## SOURCE CODE:

Compile the program using

```
javac Main.java
```

Run the program using

```
java Main
```

---

## OUTPUT:

<img width="800" height="243" alt="image" src="https://github.com/user-attachments/assets/5df587ce-7eee-47ca-86e2-f33f2326dbae" />


---

## RESULT:

Thus, the Java program to demonstrate the **class and object concept** was executed successfully and the output was verified.

----

# Ex.No:2(B) METHODS

## QUESTION:
Write a Java program to demonstrate the concept of **class and object**.

---

## AIM:
To write a Java program to demonstrate the **class and object concept using static and non-static methods**.

---

## ALGORITHM :
1. Start the program.  
2. Create a class named `Main`.  
3. Define a **static method** `printst()` to print a message.  
4. Define a **non-static method** `printnonst()` to print a message.  
5. Inside the `main()` method call the static method directly.  
6. Create an object of the class `Main`.  
7. Call the non-static method using the object.  
8. Stop the program.

---

## PROGRAM:

```java
/*
Program to implement a Class and Objects using Java
Developed by: HARI PRIYA M 
RegisterNumber: 212224240047  
*/

public class Main{
    static void printst(){
        System.out.println("I am static");
    }

    void printnonst(){
        System.out.println("I am non-static");
    }

    public static void main(String[] args){
        printst();
        Main obj = new Main();
        obj.printnonst();
    }
}
```

---

## SOURCE CODE:

Compile the program using

```
javac Main.java
```

Run the program using

```
java Main
```

---

## OUTPUT:

<img width="416" height="184" alt="image" src="https://github.com/user-attachments/assets/665be8dc-b0bf-4631-aad4-67c1449348e8" />


---

## RESULT:

Thus, the Java program to demonstrate the **class and object concept** was executed successfully and the output was verified.

----

# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to demonstrate the use of **access specifiers (private)** using getter and setter methods.

---

## AIM:
To write a Java program to demonstrate **data hiding using private access specifier with getter and setter methods**.

---

## ALGORITHM :
1. Start the program.  
2. Import the necessary package `java.util`.  
3. Create a class `BankAccount`.  
4. Declare private variables `accno` and `bal`.  
5. Create **getter methods** to return account number and balance.  
6. Create **setter methods** to set account number and balance.  
7. Create another class `prog` containing the `main()` method.  
8. Create an object of `BankAccount`.  
9. Read account number and balance from the user.  
10. Use setter methods to store values in the object.  
11. Use getter methods to display account number and balance.  
12. Stop the program.

---

## PROGRAM:

```java
/*
Program to implement a Access Specifiers using Java
Developed by: HARI PRIYA M
RegisterNumber: 212224240047
*/

import java.util.Scanner;

class BankAccount{
    private String accno;
    private double bal;
    
    public String getAccountNumber(){
        return accno;
    }
    
    public void setAccountNumber(String accno){
        this.accno = accno;
    }
    
    public double getbalance(){
        return bal;
    }

    public void setbalance(double balance){
        this.bal = balance;
    }
}

public class prog{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);

        BankAccount obj = new BankAccount();

        String tempaccno = sc.nextLine();
        double tempbal = sc.nextDouble();

        obj.setAccountNumber(tempaccno);
        obj.setbalance(tempbal);

        System.out.println("Account Number: " + obj.getAccountNumber());
        System.out.println("Balance: " + obj.getbalance());
    } 
}
```

---

## SOURCE CODE:

Compile the program using

```
javac prog.java
```

Run the program using

```
java prog
```

---

## OUTPUT:

<img width="700" height="300" alt="image" src="https://github.com/user-attachments/assets/172f8c6f-95e6-4e6f-b448-1fe29e391576" />


---

## RESULT:

Thus, the Java program to demonstrate **access specifiers using private variables and getter/setter methods** was executed successfully and the output was verified.

----

# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a Java program to demonstrate the use of **variable scope and constructor** to initialize and display employee details.

---

## AIM:
To write a Java program to demonstrate **variable scope and constructor initialization in a class**.

---

## ALGORITHM :
1. Start the program.  
2. Import the necessary package `java.util`.  
3. Create a class `Employee`.  
4. Declare variables `id`, `name`, and `salary`.  
5. Create a **constructor** to initialize these variables.  
6. Use `this` keyword to assign constructor parameters to class variables.  
7. Create a method `display()` to print employee details.  
8. Create another class `prog` containing the `main()` method.  
9. Read employee id, name, and salary from the user.  
10. Create an object of class `Employee` and pass the values to the constructor.  
11. Call the `display()` method to show employee details.  
12. Stop the program.

---

## PROGRAM:

```java
/*
Program to implement a Variable scope and Constructor using Java
Developed by: HARI PRIYA M
RegisterNumber: 212224240047
*/

import java.util.Scanner;

class Employee{
    int id;
    String name;
    double salary;
    
    public Employee(int id,String name,double salary){
        this.id = id;
        this.name = name;
        this.salary = salary;
    }
    
    public void display(){
        System.out.println("Employee Details:");
        System.out.println("Employee ID: "+id);
        System.out.println("Employee Name: "+name);
        System.out.printf("Employee Salary: %.1f",salary);
    }
}

class prog{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);

        int id = sc.nextInt();
        sc.nextLine();
        String name = sc.nextLine();
        double salary = sc.nextDouble();
        
        Employee emp = new Employee(id,name,salary);
        emp.display();
    }
}
```

---

## SOURCE CODE:

Compile the program using

```
javac prog.java
```

Run the program using

```
java prog
```

---

## OUTPUT:

```
101
Ravi Kumar
35000
Employee Details:
Employee ID: 101
Employee Name: Ravi Kumar
Employee Salary: 35000.0
```

---

## RESULT:

Thus, the Java program to demonstrate **variable scope and constructor** was executed successfully and the output was verified.

----

# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Write a Java program to demonstrate the use of **access modifiers** in a class.

---

## AIM:
To write a Java program to demonstrate **access modifiers by accessing class members through methods**.

---

## ALGORITHM :
1. Start the program.  
2. Import the necessary package `java.util`.  
3. Create a class named `Employee`.  
4. Declare a variable `name` inside the class.  
5. Create a method `setName()` to assign a value to the variable.  
6. Create a method `display()` that returns the current object using `this`.  
7. Create a method `printName()` to display the employee name.  
8. Create another class `prog` with the `main()` method.  
9. Read the employee name from the user.  
10. Create an object of class `Employee`.  
11. Call `setName()` to store the name.  
12. Call `display().printName()` to print the employee name.  
13. Stop the program.

---

## PROGRAM:

```java
/*
Program to implement a Access Modifiers using Java
Developed by: HARI PRIYA M
RegisterNumber: 212224240047
*/

import java.util.Scanner;

class Employee{
    String name;
    
    void setName(String name){
        this.name = name;
    }

    Employee display(){
        return this;
    }

    void printName(){
        System.out.println("Employee Name: " + name);
    }
}

class prog{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);

        String name = sc.nextLine();

        Employee emp = new Employee();
        emp.setName(name);

        emp.display().printName();
    }
}
```

---

## SOURCE CODE:

Compile the program using

```
javac prog.java
```

Run the program using

```
java prog
```

---

## OUTPUT:

<img width="623" height="255" alt="image" src="https://github.com/user-attachments/assets/e7f86a3e-a5f5-4e87-86e8-07a308e1f7de" />


---

## RESULT:

Thus, the Java program to demonstrate **access modifiers** was executed successfully and the output was verified.

