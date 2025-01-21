# Sum-of-digits-of-number
import java.util.Scanner;

public class SumOfDigits {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

       
        System.out.print("Enter a number: ");
        int number = scanner.nextInt();

        
        int sum = 0;
        int temp = Math.abs(number); 

        while (temp > 0) {
            int digit = temp % 10;  
            sum += digit;          
            temp /= 10;            
        }

        // Output the result
        System.out.println("The sum of digits is: " + sum);

        scanner.close();
    }
}

Output 

The sum of digits is: 10
