# Method-LoanStatus
Loan Status checker code
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println(" \n Any criminal record? True/False");
        boolean criminalRecord = scanner.nextBoolean();
        System.out.println("\n Do you have an ID card?True/False");
        boolean IdCard = scanner.nextBoolean();
        System.out.println("Please insert your saving Amount");
        Float SavingAmount = scanner.nextFloat();
        loanStatus(criminalRecord,SavingAmount,IdCard);
    }

    static void loanStatus(boolean criminalRecord,Float SavingAmount,boolean IdCard){

        String Loan = !criminalRecord && (SavingAmount>100_000 )&& (IdCard= Boolean.parseBoolean("True")) ?"Congratulation! You can take a loan.":"You cann't take a loan.";

        System.out.println("Hello Mr."+Loan);
       // return " boolean Loan";
    }
}

