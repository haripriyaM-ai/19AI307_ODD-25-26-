# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Write a Java program to demonstrate the use of variables and operators (pre-decrement and post-decrement).

## AIM:
To write a Java program to demonstrate the use of variables and decrement operators (pre and post).

## ALGORITHM :
1.	Start the program.
2.	Import the Scanner class to read input from the user.
3.	Create a class named Main.
4.	Inside the main() method, create a Scanner object.
5.	Declare an integer variable n.
6.	Read the value of n from the user.
7.	Display the initial value of n.
8.	Apply post-decrement operator (n--) and print the result.
9.	Apply pre-decrement operator (--n) and print the result
10.	Stop the program.




## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: HARI PRIYA M 
RegisterNumber: 212224240047  
*/
```

```java
import java.util.Scanner;

public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        
        System.out.println("Initial countdown = "+n);
        System.out.println("After post-decrement (a--) = "+(n--)+", Now a = "+n);
        System.out.println("After pre-decrement (--a) = "+(--n)+", Now a = "+n);
    }
}
```



## Sourcecode.java:

Compile the program using
javac Main.java

Run the program using
java Main

## OUTPUT:

<img width="978" height="295" alt="image" src="https://github.com/user-attachments/assets/662cfb16-1b23-4a4c-8438-76875fc0c33d" />




## RESULT:
Thus, the Java program to demonstrate the use of variables and decrement operators was successfully executed and the output was verified.

----

# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
Write a Java program to determine the type of triangle (Equilateral, Isosceles, Scalene) using conditional statements.

## AIM:
To write a Java program to determine the type of triangle using conditional statements.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package java.util.
3.	Create a class named Main.
4.	Inside the main() method, create a Scanner object to read input.
5.	Read three integer values representing the sides of the triangle (h, b, w).
6.	Check if the given sides satisfy the triangle condition : (h + b > w) AND (b + w > h) AND (w + h > b).
7.	If the condition is true:
   - If all three sides are equal → print Equilateral.
   - Else if any two sides are equal → print Isosceles.
   - Else → print Scalene.
8. If the triangle condition is false → print Not a triangle.

9. Stop the program.





## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: HARI PRIYA M 
RegisterNumber: 212224240047  
*/
```

```java
import java.util.Scanner;

public class Main{
    public static void main(String[] aths){
        Scanner sc = new Scanner(System.in);
        
        int h = sc.nextInt();
        int b = sc.nextInt();
        int w = sc.nextInt();
        
        if(h+b>w && b+w>h && w+h>b){
        if(h == b && b == w)System.out.println("Equilateral");
        else if(h==b || w==h ||b==w)System.out.println("Isosceles");
        else System.out.println("Scalene");
        }
        else System.out.println("Not a triangle");
    }
}

```

## SOURCE CODE:

Compile the program using
javac Main.java

Run the program using
java Main






## OUTPUT:
<img width="393" height="151" alt="image" src="https://github.com/user-attachments/assets/256ed377-6ded-4d79-bf5a-809e703dce7a" />



## RESULT:
Thus, the Java program to determine the type of triangle using conditional statements was executed successfully and the output was verified.


----

# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
Write a Java program to find the factorial of a given number using a looping statement.

## AIM:
To write a Java program to calculate the factorial of a given number using a loop.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package java.util.
3.	Create a class named Main.
4.	Inside the main() method create a Scanner object to read input.
5.	Read an integer value n from the user.
6.	Initialize a variable f to 1 to store the factorial result.
7.	Use a for loop from 1 to n.
8.	Multiply f with each number in the loop.
9.	Store the result in f.
10.	Display the factorial of the number.
11.	Stop the program.




## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: HARI PRIYA M 
RegisterNumber: 212224240047  
*/
```

```java
import java.util.Scanner;

public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int f = 1;
        
        for(int i=1;i<=n;i++){
            f = f*i;
        }
        
        System.out.println("Factorial of "+n+" is: "+f);
    }
}
```

## SOURCE CODE:

Compile the program using
javac Main.java

Run the program using
java Main






## OUTPUT:

<img width="681" height="248" alt="image" src="https://github.com/user-attachments/assets/84152090-2f71-4b81-8a32-a27112032aa9" />


## RESULT:
Thus, the Java program to find the factorial of a number using a looping statement was executed successfully and the output was verified.

----

# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java program to find the maximum odd number in an array.

## AIM:
To write a Java program to find the maximum odd number in a given array using array concept.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package java.util.
3.	Create a class named Main.
4.	Inside the main() method create a Scanner object.
5.	Read the number of elements n.
6.	Declare an array arr of size n.
7.	Use a loop to read n elements and store them in the array.
8.	Initialize a variable max with Integer.MIN_VALUE.
9.	Traverse through the array using a loop.
10.	Check if the element is odd (arr[i] % 2 != 0).
11.	If the element is odd and greater than max, update max.
12.	After the loop, check:
    - If max is still Integer.MIN_VALUE, print No odd number found.
    - Otherwise print the maximum odd number.

13. Stop the program.





## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: HARI PRIYA M 
RegisterNumber: 212224240047  
*/
```

```java
import java.util.Scanner;

public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for(int i=0;i<n;i++){
            arr[i] = sc.nextInt();
        }
        
        int max = Integer.MIN_VALUE;
        for(int i=0;i<n;i++){
            if(arr[i] % 2 !=0){
                if(arr[i] > max){
                    max = arr[i];
                }
            }
        }
        System.out.println((max == Integer.MIN_VALUE) ? "No odd number found" : max);
    }
}
```

## SOURCE CODE:

Compile the program using
javac Main.java

Run the program using
java Main




## OUTPUT:
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/cb8cfc09-32f0-49e2-bfbe-618d297832f9" />



## RESULT:
Thus, the Java program to find the maximum odd number in an array was executed successfully and the output was verified.

----

# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to find the **longest word in a given sentence**.

---

## AIM:
To write a Java program to **identify the longest word from a given string using string functions**.

---

## ALGORITHM :
1. Start the program.  
2. Import the necessary package `java.util`.  
3. Create a class `Main`.  
4. Inside the `main()` method create a `Scanner` object.  
5. Read a full line string from the user.  
6. Split the string into words using `split("\\s+")`.  
7. Store the first word as the longest word.  
8. Traverse through the remaining words using a loop.  
9. Compare the length of each word with the current longest word.  
10. If a word is longer, update the longest word.  
11. Display the longest word.  
12. Stop the program.

---

## PROGRAM:

```java
/*
Program to find the longest word in a string
Developed by: HARI PRIYA M
RegisterNumber: 212224240047
*/

import java.util.Scanner;

public class Main
{
    public static void main(String args[])
    {
        Scanner sc=new Scanner(System.in);

        String a=sc.nextLine();

        String[] words=a.split("\\s+");

        String l=words[0];
        
        for(int i=1;i<words.length;i++)
        {
            if(words[i].length()>l.length())
            {
                l=words[i];
            }
        }

        System.out.println("The longest word is: "+l);
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

<img width="747" height="261" alt="image" src="https://github.com/user-attachments/assets/342723c1-b57f-44c9-8b13-95771e3cf7c6" />


---

## RESULT:

Thus, the Java program to find the **longest word in a given string** was executed successfully and the output was verified.

