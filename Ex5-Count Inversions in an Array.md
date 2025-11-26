# Ex5 Count Inversions in an Array
## DATE:26-11-2025
## AIM:
To write a Java program  to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j

## Algorithm:
 1.Start the program.
 
 2.Read the number of elements and store them in an array.
 
 3.Use a modified merge sort to count inversions: .Recursively split the array into halves and count  inversions in each half. .While merging two sorted halves,
 
 4.count cross inversions when an element from the right half is placed before elements remaining in the left half.
 
 5.Sum inversions from left half, right half, and cross inversions.
 
 6.Display the total inversion count.
 
 7.Stop the program.
## Program:
```
/*
Program toto Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j
Developed by:  VEDHASHREE G
RegisterNumber:  212223240171

 import java.util.Scanner;
 public class CountInversions {
 public static void main(String[] args) {
 Scanner sc = new Scanner(System.in);
 int n = sc.nextInt();
 int[] arr = new int[n];
 for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
        long result = mergeSortAndCount(arr, 0, n - 1);
        System.out.println(result);
    }
    private static long mergeSortAndCount(int[] arr, int left, int right) {
        long count = 0;
        if (left < right) {
            int mid = (left + right) / 2;
            count += mergeSortAndCount(arr, left, mid);
            count += mergeSortAndCount(arr, mid + 1, right);
            count += mergeAndCount(arr, left, mid, right);
        }
        return count;
    }
    private static long mergeAndCount(int[] arr, int left, int mid, int right) {
        int[] leftArr = new int[mid - left + 1];
        int[] rightArr = new int[right - mid];
        System.arraycopy(arr, left, leftArr, 0, leftArr.length);
        System.arraycopy(arr, mid + 1, rightArr, 0, rightArr.length);
        int i = 0, j = 0, k = left;
        long swaps = 0;
        while (i < leftArr.length && j < rightArr.length) {
            if (leftArr[i] <= rightArr[j]) {
                arr[k++] = leftArr[i++];
            } else {
                arr[k++] = rightArr[j++];
                swaps += (mid + 1) - (left + i);
            }
        }
        while (i < leftArr.length) {
            arr[k++] = leftArr[i++];
        }
        while (j < rightArr.length) {
            arr[k++] = rightArr[j++];
        }
        return swaps;
    }
 }

*/
```

## Output:

<img width="1212" height="386" alt="image" src="https://github.com/user-attachments/assets/bdd8fac3-baa8-49e3-ab89-15d6c75ce670" />


## Result:
Thus the Java program to to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < jis implemented successfully.
