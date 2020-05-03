
Input
3

Output
  #
 ##
###

```java
import java.util.Scanner;

public class StairCase {
    static void staircase(int n) {
        String asteriks = "#";
        for (int row = 0; row < n; row++) {
            System.out.printf("%"+(n)+"s%n", asteriks);
            asteriks += "#";
        }
    }

    private static final Scanner scanner = new Scanner(System.in);

    public static void main(String[] args) {
        int n = scanner.nextInt();
        scanner.skip("(\r\n|[\n\r\u2028\u2029\u0085])?");

        staircase(n);

        scanner.close();
    }
}
```
