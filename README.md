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
2) Rotate the characters in a string by a given input and have the overflow appear at the beginning, e.g. “MyString” rotated by 2 is “ngMyStri”.

```
public static void rotate(String s, int rotation) {
        rotation %= s.length(); 
        String ending = s.substring((s.length() - rotation), s.length());
        String remainder = s.substring(0, s.length() - rotation); 
        System.out.println(ending + remainder);
     }

```

3) If you could change 1 thing about your favorite framework/language/platform (pick one), what would it be?
```
My favorite framework at the moment is angular, I would love it if the developers could simplify forms. 
I think they have come a long way, but I see their current solution of making a service to instantiate 
with the validator and control name to be overly repetitive and somewhat over engineered. I believe that 
in that scenario, where most of the time they are used the same way, there should be a very simple 
interface to hook into that can output value without any setup.
```
