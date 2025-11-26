# Ex4 You are given a Java program that performs matrix addition. If Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension, what will be the nature (even/odd/mixed) of the resulting matrix?
## DATE:26-11-2025
## AIM:
-To write a java function to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix.-
## Algorithm:
 1.Start the program.
 
 2.Read the dimensions of both matrices (rows and columns). Check whether Matrix A and Matrix B
 
 have the same dimensions. If not, display “Matrices are not of same dimension” and stop.
 
 3.Read Matrix A and check each element: If every element is odd, continue.
 
 4.If any element is even, mark A as invalid and stop further checking.
 
 5.Read Matrix A and check each element: If every element is odd, continue.
 
 6.If any element is even, mark A as invalid and stop further checking.
 
 7.If both matrices are valid, compute the resultant matrix (e.g., A + B or any operation specified).

 Determine the nature of the resultant matrix:
 
 8.If all elements are odd, print “Resultant matrix is an Odd Matrix”.
 
 9.If all elements are even, print “Resultant matrix is an Even Matrix”. Otherwise, print “Resultant matrix is a Mixed Matrix”.
 
 10.Display the Resultant Matrix.
 
 11.Stop the program
## Program:
```
/*
Program to ind the nature of resultant matrrix.
Developed by: 
RegisterNumber:
 import java.util.Scanner;
 public class MatrixAddition {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int rows = sc.nextInt();
        int cols = sc.nextInt();
        int[][] A = new int[rows][cols];
        int[][] B = new int[rows][cols];
        int[][] result = new int[rows][cols];
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                A[i][j] = sc.nextInt();
            }
        }
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                B[i][j] = sc.nextInt();
            }
        }
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                result[i][j] = A[i][j] + B[i][j];
            }
        }
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                System.out.print(result[i][j] + " ");
            }
            System.out.println();
        }
       
    }
 }
*/
```

## Output:
<img width="329" height="480" alt="image" src="https://github.com/user-attachments/assets/5c59a01a-9a12-46b8-8c94-bb9c66c450d9" />

## Result:
Thus, the java program to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix is implemented successfully.
