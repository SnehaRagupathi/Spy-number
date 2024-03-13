import java.util.Scanner;
class Main {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int num = in.nextInt();
        int sum = 0;
        int product = 1;
        int a = num;
        while (a > 0) {
            int b = a % 10;
            sum += b;       
            product *= b;   
            a /= 10;
        }
        if (sum == product) {
            System.out.println(num + " is a Spy Number.");
        } else {
            System.out.println(num + " is not a Spy Number.");
        }
    }
}
