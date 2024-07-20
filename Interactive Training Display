import java.util.Scanner;

public class MenuProgram {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int choice;

        while (true) {
            displayMenu();
            System.out.print("Enter your choice: ");
            if (!scanner.hasNextInt()) {
                System.out.println("Invalid input. Please enter a number.");
                scanner.next(); // Clear the invalid input
                continue;
            }
            choice = scanner.nextInt();

            switch (choice) {
                case 1:
                    displayRightAngleTriangle(scanner);
                    break;
                case 2:
                    displayPalindromicTriangle(scanner);
                    break;
                case 3:
                    displayHelp();
                    break;
                case 4:
                    System.out.println("Exiting the program. Goodbye!");
                    return;
                default:
                    System.out.println("Invalid choice. Please enter a number between 1 and 4.");
            }
        }
    }

    private static void displayMenu() {
        System.out.println("Menu:");
        System.out.println("1. Display a right-angle triangle of ones");
        System.out.println("2. Display a Palindromic Triangle");
        System.out.println("3. Help");
        System.out.println("4. Exit");
    }

    private static void displayRightAngleTriangle(Scanner scanner) {
        System.out.print("Enter the number of lines: ");
        int lines = scanner.nextInt();

        for (int i = 1; i <= lines; i++) {
            // Print ascending numbers
            for (int j = 1; j <= i; j++) {
                System.out.print(j);
            }
            // Print descending numbers
            for (int j = i - 1; j >= 1; j--) {
                System.out.print(j);
            }
            System.out.println();
        }
    }

    private static void displayPalindromicTriangle(Scanner scanner) {
        System.out.print("Enter the number of lines: ");
        int lines = scanner.nextInt();

        for (int i = 1; i <= lines; i++) {
            // Print spaces
            for (int j = i; j < lines; j++) {
                System.out.print(" ");
            }
            // Print descending numbers
            for (int j = i; j >= 1; j--) {
                System.out.print(j);
            }
            // Print ascending numbers
            for (int j = 2; j <= i; j++) {
                System.out.print(j);
            }
            System.out.println();
        }
    }

    private static void displayHelp() {
        System.out.println("Help:");
        System.out.println("1. Display a right-angle triangle of ones: Prompts for the number of lines and displays a right-angle triangle of ones.");
        System.out.println("2. Display a Palindromic Triangle: Prompts for the number of lines and displays a palindromic triangle.");
        System.out.println("3. Help: Displays this help information.");
        System.out.println("4. Exit: Exits the program.");
    }
}
