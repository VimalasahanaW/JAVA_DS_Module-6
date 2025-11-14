# EX 1 You’re creating a health monitoring device which stores several sensor readings in an array. To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
## DATE: 14-11-12
## AIM:
To write a JAVA program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.

## Algorithm
1. Start with the array and begin at the first element.
2.If you are at the last element, return that value.
3.Otherwise, find the minimum value in the rest of the array using recursion.
4.Compare the current element with the minimum of the remaining elements.
5.Return the smaller value as the minimum.
   

## Program:
```
/*
Program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
Developed by: VIMALA SAHANA W
RegisterNumber: 212223040241
*/
public class HealthMonitor {

    // Recursive method to find minimum value in the array
    public static int findMin(int[] arr, int index) {
        // Base case: if last element, return it
        if (index == arr.length - 1) {
            return arr[index];
        }

        // Recursive case: find minimum in the rest of the array
        int minOfRest = findMin(arr, index + 1);

        // Compare current element with minimum of remaining elements
        return Math.min(arr[index], minOfRest);
    }

    public static void main(String[] args) {
        int[] heartBeats = {78, 85, 90, 72, 88, 76};

        int minimumValue = findMin(heartBeats, 0);

        System.out.println("Lowest Heartbeat Reading: " + minimumValue);
    }
}

```

## Output:
<img width="419" height="106" alt="image" src="https://github.com/user-attachments/assets/3ca92196-d53c-4d6f-beb7-fc8013a42d0f" />



## Result:
Thus the JAVA program to  find the minimum value (e.g., lowest heartbeat), implement a recursive method has implemented successfully.
