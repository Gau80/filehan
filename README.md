import java.util.Scanner;

public class filehandling2 {
    public static void main(String[] args) {
        int sum = 0;
        try(Scanner s = new Scanner(System.in)) {

            int[] arr = new int[5];
            System.out.println("Enter the elements");
            for (int i = 0; i < 5; i++) {
                int ele = s.nextInt();
                arr[i] = ele;
                ele = 0;

                sum = sum + arr[i];

            }
            System.out.println("The Sum of numbers are="+' '+ ' '+ sum);
            System.out.println("the average of elements" + ' ' + (sum/5) );
        } catch (ArithmeticException|InputMismatchException e) {
            System.out.println(e);
        }
        System.out.println("Go to hell");
    }
}
