import java.util.Scanner;
import java.util.Random;

public class GuessTheNumber {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Random random = new Random();
        int secretNumber;
        int guess;
        int attempts;
        int maxAttempts = 5;
        String playAgain;

        System.out.println("Welcome to the Guess the Number game!");

        do {
            secretNumber = random.nextInt(100) + 1; // Step 1

            attempts = 0;
            while (attempts < maxAttempts) { // Step 5
                System.out.print("Guess the number (between 1 and 100): ");
                guess = scanner.nextInt();
                attempts++;

                if (guess < secretNumber) {
                    System.out.println("Too low! Try again."); // Step 3
                } else if (guess > secretNumber) {
                    System.out.println("Too high! Try again."); // Step 3
                } else {
                    System.out.println("Congratulations! You've guessed the number " + secretNumber + " correctly in " + attempts + " attempts!");
                    break;
                }
            }

            if (attempts == maxAttempts) {
                System.out.println("Sorry, you've run out of attempts! The number was " + secretNumber + "."); // Step 3
            }

            System.out.print("Do you want to play again? (yes/no): ");
            playAgain = scanner.next().toLowerCase();
        } while (playAgain.equals("yes")); // Step 6

        System.out.println("Thanks for playing!");
        scanner.close();
    }
}
