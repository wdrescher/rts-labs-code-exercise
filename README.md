### RTS Coding Exercise

1)  Print the number of integers in an array that are above the given input and the number that are below, e.g. for the array [1, 5, 2, 1, 10] with input 6, print “above: 1, below: 4”.


```
public static void pivot(int [] arr, int input) {
         int above = 0; 
         int below = 0; 
         for (int i = 0; i < arr.length; i++) {
             if (arr[i] < input) {
                 below++; 
             }
             else if (arr[i] > input) {
                 above++; 
             }
         }
         System.out.println("above: " + above + ", below: " + below);
  }

```
