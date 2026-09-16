# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
A pirate ship has a code lock that only opens if:

1)The input code is even, and

2)If it is less than 100, say "Weak Code".

3)If it is between 100 and 999, say "Strong Code".

4)If the code is odd, deny access.


## AIM:
To write a Java program that accepts a code number and determines the security level based on the given conditions:

If the code is even and less than 100 → Display "Weak Code"
If the code is even and between 100 and 999 → Display "Strong Code"
Otherwise → Display "Access Denied"


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read an integer value from the user and store it in variable 'code'.
4.Check if 'code' is even (code % 2 == 0): a. If 'code' is less than 100: - Print "Weak Code". b. Else if 'code' is between 100 and 999 (inclusive): - 5.Print "Strong Code". c. Else: - Print "Access Denied".
6.If 'code' is odd:
7.Print "Access Denied".
8.End the program.





## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: DHARSHANA A S
RegisterNumber: 212224220022
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class PirateCodeLock {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int code = sc.nextInt();

        if (code % 2 == 0) {
            if (code < 100) {
                System.out.println("Weak Code");
            } else if (code >= 100 && code <= 999) {
                System.out.println("Strong Code");
            }
            else
            {
                System.out.println("Access Denied");
            }
        } else {
            System.out.println("Access Denied");
        }
    }
}

```






## OUTPUT:
<img width="1253" height="395" alt="image" src="https://github.com/user-attachments/assets/7136cd63-3247-40ff-9535-fd79dbc70465" />




## RESULT:
Therefore,the program has been executed successfully.
