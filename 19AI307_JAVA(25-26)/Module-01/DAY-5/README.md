# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to remove spaces from a given string using string functions.

## AIM:
To write a Java program to remove all spaces from a given string using string functions.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package java.util.
3.	Create a class named Main.
4.	Inside the main() method create a Scanner object.
5.	Read a string input from the user using nextLine().
6.	Use the replaceAll() method to remove spaces from the string.
7.	Store the modified string in a variable.
8.	Display the string without spaces.
9.	Stop the program.	





## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: HARI PRIYA M 
RegisterNumber: 212224240047  
*/
```
```java
import java.util.Scanner;

public class Main{
    public static void main(String[] ars){
        Scanner ac = new Scanner(System.in);
        String str = ac.nextLine().replaceAll(" ","");
        System.out.println("String without spaces: "+str);
    }
}
```

## SOURCE CODE:
Compile the program using
javac Main.java

Run the program using
java Main







## OUTPUT:
```
Hello World Java
String without spaces: HelloWorldJava
```


## RESULT:
Thus, the Java program to remove spaces from a given string using string functions was executed successfully and the output was verified.
