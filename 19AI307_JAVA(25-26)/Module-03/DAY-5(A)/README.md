# Ex.No:3(E) INNER CLASS

## QUESTION:
Write a Java program to demonstrate the concept of **Inner Class** by checking whether a number is prime or not.

---

## AIM:
To write a Java program to demonstrate the **Inner Class concept**.

---

## ALGORITHM :
1. Start the program.  
2. Import the necessary package `java.util`.  
3. Create a class `Main`.  
4. Inside `Main`, create an **inner class `PrimeChecker`**.  
5. Define a method `checkPrime(int n)` inside the inner class.  
6. In the method, check if the number is prime using a loop from `2` to `√n`.  
7. In the `main()` method create a `Scanner` object.  
8. Read the input from the user.  
9. Convert the input string into an integer using `Integer.parseInt()`.  
10. Create an object of the inner class `PrimeChecker`.  
11. Call the method to check whether the number is prime or not.  
12. Handle invalid input using `try-catch`.  
13. Stop the program.

---

## PROGRAM:

```java
/*
Program to implement Inner Class using Java
Developed by: HARI PRIYA M
RegisterNumber: 212224240047
*/

import java.util.Scanner;

public class Main{

    // Inner Class
    class PrimeChecker{

        void checkPrime(int n){
            if(n <= 1){
                System.out.println(n + " is not a prime number.");
                return;
            }

            boolean isPrime = true;

            for(int i = 2; i <= Math.sqrt(n); i++){
                if(n % i == 0){
                    isPrime = false;
                    break;
                }
            }

            if(isPrime)
                System.out.println(n + " is a prime number.");
            else
                System.out.println(n + " is not a prime number.");
        }
    }

    public static void main(String[] args){

        Scanner sc = new Scanner(System.in);
        Main obj = new Main();

        String num = sc.nextLine();

        try{
            int n = Integer.parseInt(num);

            PrimeChecker pc = obj.new PrimeChecker();
            pc.checkPrime(n);

        }catch(NumberFormatException e){
            System.out.println("Invalid input. Please enter a valid integer.");
        }

        sc.close();
    }
}
```

---

## OUTPUT:
<img width="609" height="225" alt="image" src="https://github.com/user-attachments/assets/0c77b4dd-5f14-47ff-b9e5-26ec4b890b6f" />


---

## RESULT:

Thus, the Java program to demonstrate the **Inner Class concept** was executed successfully and the output was verified.
