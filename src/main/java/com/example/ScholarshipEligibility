import java.util.Scanner;

public class ScholarshipEligibility {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Input details
        System.out.print("Enter your Category (General, OBC, SC, ST): ");
        String category = scanner.next().toUpperCase();

        System.out.print("Enter your Marks (Percentage): ");
        double marks = scanner.nextDouble();

        System.out.print("Enter Annual Family Income: ");
        double income = scanner.nextDouble();

        // Check Eligibility
        boolean isEligible = false;
        String scheme = "";

        if (category.equals("SC") || category.equals("ST")) {
            if (marks >= 50 && income <= 250000) {
                isEligible = true;
                scheme = "Post-Matric SC/ST Scholarship";
            }
        } else if (category.equals("OBC")) {
            if (marks >= 60 && income <= 150000) {
                isEligible = true;
                scheme = "OBC Merit-cum-Means Scholarship";
            }
        } else if (category.equals("GENERAL")) {
            if (marks >= 75 && income <= 100000) {
                isEligible = true;
                scheme = "EWS/General Merit Scholarship";
            }
        }

        // Output Result
        if (isEligible) {
            System.out.println("Congratulations! You are eligible for: " + scheme);
        } else {
            System.out.println("Sorry, you do not meet the criteria for standard schemes.");
        }
        
        scanner.close();
    }
}
