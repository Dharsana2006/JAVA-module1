# Module-1
# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely is training to become a logic wizard. She enters a gate that tests her understanding of logical conditions.

She is given two magical conditions:

hasKey – whether she has the golden key (boolean)

knowsPassword – whether she knows the secret password (boolean)

The gate then evaluates her truthfulness using logical operators:

<img width="390" height="134" alt="image" src="https://github.com/user-attachments/assets/0660b40a-98a0-47bd-9151-2abc1a08e17d" />

Write a program that:

Accepts two boolean inputs: hasKey and knowsPassword

Displays the results of:

hasKey && knowsPassword
hasKey || knowsPassword
!hasKey
!knowsPassword
**Input Format:**

First line: true or false (hasKey)

Second line: true or false (knowsPassword)

**Output Format:**

Access with AND: <true/false>

Access with OR: <true/false>

Does NOT have key: <true/false>

Does NOT know password: <true/false>

## AIM:
Aim:
To write a Java program that reads two integer numbers from the user and performs basic arithmetic operations such as addition, subtraction, multiplication, division, and modulus, and displays the results.


## ALGORITHM :
1. Start
2. Create a Scanner object to read input from the user.
3. Read two boolean values i and j from the user.
4. Compute the following:
       l1 = i && j → Logical AND of i and j
   
       l2 = i || j → Logical OR of i and j
   
       l3 = !i → Logical NOT of i
   
       l4 = !j → Logical NOT of j
   
5.Display the results:

      "Access with AND: " + l1

      "Access with OR: " + l2

       "Does NOT have key: " + l3

      "Does NOT know password: " + l4

6. Stop



## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: Dharsana A
RegisterNumber:  212224060061
*/
```

## Sourcecode.java:
```
import java.util.*;
public class Main{
    public static void main(String[]args)
    {
        Scanner sc=new Scanner(System.in);
        boolean i=sc.nextBoolean();
        boolean j = sc.nextBoolean();
        boolean l1=(i&&j);
        boolean l2=(i||j);
        boolean l3=(!i);
        boolean l4=(!j);
        System.out.println("Access with AND: "+l1);
        System.out.println("Access with OR: "+l2);
        System.out.println("Does NOT have key: "+l3);
        System.out.println("Does NOT know password: "+l4);
    }
}
```


## OUTPUT:

<img width="848" height="415" alt="image" src="https://github.com/user-attachments/assets/47e4fe9b-ed37-4b1f-a010-fd6bb9f111fb" />



## RESULT:

The program has been executed successfully and the desired output has been obtained.



# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
Aliens scan DNA numbers:

If the DNA number is divisible by 2 and ends in 4, they accept it.

If the DNA number is divisible by 2 but ends in anything else, it’s a suspect.

If the DNA is odd, they reject it.

## For example:

```
---------------------------
Input	       Result 
64        |  Accepted
-----------------------------

```
## AIM:

To implement conditional logic in Java using nested if-else statements and the modulus operator to solve a classification problem.


## ALGORITHM :

1.Start the program.

2.Import the java.util.Scanner class for user input.

3.Create a Scanner object to read from the console.

4.Read the integer dnaNumber from the user.

5.Check if dnaNumber is even ( dnaNumber % 2 == 0 ).

6.If it is even, enter a nested check:

7.Check if dnaNumber ends in 4 ( dnaNumber % 10 == 4 ).

  - If true, print "Accepted".

  - If false, print "Suspect".

  - If the number is not even (it's odd), print "Rejected".

8. End the program.


## PROGRAM:
 ```

Program to implement a conditional statement using Java
Developed by:  Dharsana A
RegisterNumber:  212224060061

```

## SOURCE CODE:

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int dnaNumber = scanner.nextInt();

        if (dnaNumber % 2 == 0) {
            if (dnaNumber % 10 == 4) {
                System.out.println("Accepted");
            } else {
                System.out.println("Suspect");
            }
        } else {
            System.out.println("Rejected");
        }

    }
}
```


## OUTPUT:

<img width="1235" height="476" alt="Screenshot 2025-11-16 123601" src="https://github.com/user-attachments/assets/d34b3a42-80cd-4c93-a256-f74f86f91358" />


## RESULT:


The program was successfully developed and executed.It correctly classifies the given DNA number as Accepted, Suspect, or Rejected based on the specified conditional rules.



# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
Construct a right-angled triangle star pattern using for loop.
## AIM:
To write a Java program using looping statements to print a right-angled triangle star pattern based on user input.

## ALGORITHM :
1.	Start the program.

2.	Import the necessary package 'java.util'

3. Read the number of rows from the user.

4. Use an outer loop to iterate through each row.

5. Use an inner loop to print stars (*) for each row.

6. Move to the next line after printing stars for each row.

7. End the program.


## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: Dharsana a
Register Number: 212224060061
*/
```

## SOURCE CODE:

```java
import java.util.*;
public class TrianglePattern
{
    public static void main(String args[])
    {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        for (int i = 1; i <= n; i++) 
        {         
            for (int j = 1; j <= i; j++) 
            {      
                System.out.print("* ");
            }
            System.out.println();              
        }
    }
}
```

## OUTPUT:
<img width=30% src="https://github.com/user-attachments/assets/07286d0c-5174-4702-8d58-34b630bd23d6" />

## RESULT:
Thus, the Java program using looping statements to print a right-angled triangle star pattern was successfully written, executed, and verified.


# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java program to check whether an element appears more than once in an array.

## AIM:
To write a Java program that uses arrays and a data structure (HashSet) to check if any element is repeated in the given array.

## ALGORITHM :
1. Start the program.
2. Import the java.util package.
3. Read the size of the array (n) from the user.
4. Create an integer array of size n.
5. Read n elements from the user and store them in the array.
6. Create a HashSet to track seen elements.
7. Traverse each element in the array.
8. If an element is already in the HashSet, mark duplicate as true and stop checking.
9. Otherwise, add the element to the HashSet.
10. After traversal, if a duplicate was found, print "Yes"; otherwise print "No".
11. End the program.



## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: Dharsana A
RegisterNumber:  212224060061
*/
```

## SOURCE CODE:

```
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for(int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        boolean duplicate = false;
        Set<Integer> seen = new HashSet<>();
        for(int num : arr) {
            if(seen.contains(num)) {
                duplicate = true;
                break;
            }
            seen.add(num);
        }

        if(duplicate)
            System.out.println("Yes");
        else
            System.out.println("No");
    }
}



```





## OUTPUT:

<img width="610" height="726" alt="image" src="https://github.com/user-attachments/assets/a2f1dfdf-35db-4c77-a9cf-005c029da767" />



## RESULT:
  Thus, the Java program was successfully written and executed to check whether any element appears more than once in an array.


# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to find the absolute value of a number using Math.abs().

## AIM:
To write a Java program that finds the absolute value of a given number using the Math.abs() method.

## ALGORITHM :
1.Start the program and create a Scanner object.

2.Read a number n (can be integer or decimal) from the user.

3.Use the built-in function Math.abs(n) to compute its absolute value.

4.Display the calculated absolute value.

5.End the program.



## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: Dharsana A
Register Number:212224060061
*/
```


## SOURCE CODE:
```
import java.util.*;
public class demo
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        double n=sc.nextDouble();
        System.out.println("Absolute value = "+Math.abs(n));
    }
}
```


## OUTPUT:
<img width="744" height="288" alt="image" src="https://github.com/user-attachments/assets/5fab9f43-7f0e-491d-bbad-5c3b7979703e" />



## RESULT:
Therefore the program successfully reads a number and calculates its absolute value.



