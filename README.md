# Armstrong
import java.util.Scanner;
public class Armstrong {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int r;
        int sum = 0;
        int temp = n;
        while (n > 0) {
            r = n % 10;
            sum = sum + r * r * r;
            n = n / 10;
        }
        if (temp == sum) {
            System.out.println("is a armstrong number");
        } else {
            System.out.println("is not a armstrong number");
        }
    }
}

