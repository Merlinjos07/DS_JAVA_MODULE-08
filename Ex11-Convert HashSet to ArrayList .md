# Ex11 Convert HashSet to ArrayList in Java
## DATE:3.8.2026
## AIM:
To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
## Algorithm
Start the program. Create a HashSet to store a collection of distinct integers. Add a few integers to the HashSet. Create an ArrayList and initialize it with the elements of the HashSet. Display the elements of both HashSet and ArrayList and End the program.
## Program:
```
/*
Program to To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
Developed by: MERLIN M
RegisterNumber:  212225240084
*/
import java.util.*;

public class HashSetToArrayList {

    public static ArrayList<Integer> convertToArrayList(HashSet<Integer> set) {
        ArrayList<Integer> list = new ArrayList<>(set);
        return list;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        HashSet<Integer> set = new HashSet<>();
        for (int i = 0; i < n; i++) {
            int num = sc.nextInt();
            set.add(num);
        }

        ArrayList<Integer> list = convertToArrayList(set);
        System.out.println("ArrayList contents:");
        for (int num : list) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}
```

## Output:
<img width="642" height="682" alt="image" src="https://github.com/user-attachments/assets/33d5bc36-e675-4138-b4c7-3bf43ce7e0a4" />



## Result:
The program successfully converts a collection of distinct integers stored in a HashSet into an ArrayList
