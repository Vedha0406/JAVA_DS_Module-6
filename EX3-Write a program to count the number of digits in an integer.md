# EX3 Write a program to count the number of digits in an integer.
## DATE:26-11-2025
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
 1.Start the program.
 
 2.Read an integer from the user.
 
 3.Define a recursive function countDigits() that counts digits by dividing the number by 10 each time.
 
 4.Base condition: if the number is 0, return 0.
 
 5.Recursive step: return 1 + countDigits(number / 10).
 
 6.Display the total count of digits. 7.Stop the program.

## Program:
```
/*
Program to to count the number of digits in an integer
Developed by: VEDHASHREE G
RegisterNumber: 212223240171

 import java.util.Scanner;
 public class CountDigits {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
     
        int num = sc.nextInt();
        
        int count = 0;
        int n = Math.abs(num); 
        
        
        if (n == 0) {
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
            count = 1;
        } else {
            while (n > 0) {
                n = n / 10;  
                count++;
            }
        }
        
        System.out.println("Number of digits: " + count);
        sc.close();
    }
 }
*/
```

## Output:
<img width="779" height="312" alt="image" src="https://github.com/user-attachments/assets/dff69d7b-be44-4a52-b6f8-1d62cd1c019e" />

## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
