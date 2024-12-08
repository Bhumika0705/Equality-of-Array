# Equality-of-Array
it will check equality of array
import java.util.Scanner;

public class EqualityofArray {
    public EqualityofArray() {
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the no. of Elements in Array: ");
        int n = sc.nextInt();
        int[] arr1 = new int[n];
        int[] arr2 = new int[n];

        for(int i = 0; i < n; ++i) {
            arr1[i] = sc.nextInt();
        }

        boolean ans = true;

        for(int i = 0; i < n; ++i) {
            arr2[i] = sc.nextInt();
            if (arr2 != arr1) {
                ans = false;
                break;
            }
        }

        System.out.println(ans);
    }
}
