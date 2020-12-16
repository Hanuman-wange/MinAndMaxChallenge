# MinAndMaxChallenge
This is one of my practice exercise of Java on Min and Max challenge. This program takes input of type Integer till a invalid input is entered and returns the maximum &amp; Minimum value
public class Main {

    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        int min = Integer.MAX_VALUE;
        int max = Integer.MIN_VALUE;
        while(true) {

            System.out.println("Enter number:");
            boolean isAnInt = scanner.hasNextInt();

            if(isAnInt) {

                int number = scanner.nextInt();

                if(number > max) {
                    max = number;
                }

                if(number < min) {
                    min = number;
                }

            } else {
                break;
            }
            scanner.nextLine(); // handle input
        }
        System.out.println("min= "+ min + ", max= " + max);
        scanner.close();
    }
}
