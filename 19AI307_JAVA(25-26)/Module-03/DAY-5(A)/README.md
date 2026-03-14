# Ex.No:3(E) INNER CLASS

## QUESTION:
Write a Java program to check whether a given number is **prime or not** and handle **invalid input using exception handling**.

---

## AIM:
To write a Java program to **check whether a number is prime or not and handle invalid inputs**.

---

## ALGORITHM :
1. Start the program.  
2. Import the necessary package `java.util`.  
3. Create a class `Main`.  
4. Inside the `main()` method create a `Scanner` object.  
5. Read the input as a string.  
6. Convert the string into an integer using `Integer.parseInt()`.  
7. If the number is less than or equal to 1, print that it is not a prime number.  
8. Otherwise check divisibility from `2` to `√n`.  
9. If any number divides `n`, mark it as not prime.  
10. If no divisor is found, print that the number is prime.  
11. Use `try-catch` block to handle invalid integer input.  
12. If an exception occurs, print an invalid input message.  
13. Stop the program.

---

## PROGRAM:

```java
/*
Program to implement a InnerClass using Java
Developed by: HARI PRIYA M
RegisterNumber: 212224240047
*/

import java.util.Scanner;

public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);

        String num = sc.nextLine();
        
        try{
            Integer n = Integer.parseInt(num);
            
            if(n <= 1){
                System.out.println(n + " is not a prime number.");
            }else{
                boolean isprime = true;

                for(int i = 2; i <= Math.sqrt(n); i++){
                    if(n % i == 0){
                        isprime = false;
                        break;
                    }
                }
                
                if(isprime){
                    System.out.println(n + " is a prime number.");
                }else{
                    System.out.println(n + " is not a prime number.");
                }
            }
        
        }catch(NumberFormatException e){
            System.out.println("Invalid input. Please enter a valid integer.");
        }

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

```
7
7 is a prime number.
```

(or)

```
10
10 is not a prime number.
```

(or)

```
abc
Invalid input. Please enter a valid integer.
```

---

## RESULT:

Thus, the Java program to **check whether a number is prime or not with exception handling** was executed successfully and the output was verified.
