# Question-Three
Assignment
// This program helps kids learn divisibly test of numbers of integers.
// The program checks whether the given integer is divisible by integers in the range of 0-9.

import java.util.Scanner;

public class DivisibilityTest {

    public static void main(String[] args) {

        // Create a Scanner object to read user input.
        Scanner scanner = new Scanner(System.in);

        // Ask the user to enter a number.
        System.out.println("Enter a number: ");
        int number = scanner.nextInt();

        // Check if the number is divisible by 0-9.
        for (int i = 0; i < 10; i++) {
            if (number % i == 0) {
                // The number is divisible by i.
                System.out.println("The number is divisible by " + i + " because it ends with a " + (i == 0 ? "zero" : i));
            }
        }
    }
}
