# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION:
Maintain two int variables a and b, read their initial values from user. Use synchronized block to swap them and print swapped values.

## AIM:
To write a Java program that reads two integers from the user and swaps their values using a synchronized block to ensure thread-safe operations.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read two integer values a and b from the user.

4.Create a lock object to use inside the synchronized block.

5.Enter the synchronized block using the lock object.

6.Swap the values of a and b using a temporary variable.

7.Exit the synchronized block once the swap is complete.

8.Print the swapped values of a and b.

9.Close the scanner.





## PROGRAM:
 ```
/*
Program to implement a Synchronization concept using Java
Developed by: DHARSHANA A S
RegisterNumber:  212224220022
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class SwapUsingSynchronized {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        Object lock = new Object();

        synchronized (lock) {
            int temp = a;
            a = b;
            b = temp;
        }

        System.out.println("a = " + a);
        System.out.println("b = " + b);
        sc.close();
    }
}
```
## OUTPUT:
<img width="457" height="390" alt="image" src="https://github.com/user-attachments/assets/d28e5471-b3a6-4b3b-b165-bde83de68033" />



## RESULT:
Therefore the program successfully swaps two integers within a synchronized block, ensuring safe and controlled access.
