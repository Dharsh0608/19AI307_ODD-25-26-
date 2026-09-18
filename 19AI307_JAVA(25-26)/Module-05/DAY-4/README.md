# Ex.No:5(D) THREAD PRIORITY

## QUESTION:
Write a Java program to implement a extending thread class

## AIM:
To write a Java program that demonstrates multithreading by creating a user-defined thread class that extends Thread and executes its own run() method.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a class MyThread that extends the Thread class.

4.Override the run() method to print numbers from 1 to 5.

5.In the main() method: Print a message indicating the main thread execution.

6.Create an instance of MyThread.

7.Call the start() method to begin execution in a separate thread.

8.Allow the thread to run independently from the main thread.





## PROGRAM:
 ```
/*
Program to implement a Thread Priority Concept using Java
Developed by: DHARSHANA A S
RegisterNumber: 212224220022 
*/
```

## SOURCE CODE:
```
public class MyThread extends Thread {
    public void run() {
        for (int i = 1; i <= 5; i++) {
            System.out.println("Thread: " + i);
        }
       
    }

    public static void main(String[] args) {
        System.out.println("Main thread finished");
        MyThread t = new MyThread();
        t.start();
    }
}
```


## OUTPUT:
<img width="612" height="355" alt="image" src="https://github.com/user-attachments/assets/eb417c14-dc73-4224-863a-54bbc5955877" />



## RESULT:
Therefore the program successfully creates a separate thread by extending Thread and executes the overridden run() method.
