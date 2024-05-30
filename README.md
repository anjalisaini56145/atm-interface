# atm-interface
import java.util.*;
public class atm_interface {
    public static void main(String[] args) {
        int balance = 100000, WITHDRAW ,DEPOSITE;
        Scanner sc = new Scanner(System.in);
        // GIVE CHOICE TO THE USER 
        System.out.println(" WELCOME TO ATM");
        System.out.println("choose 1 for DEPOSITE");
        System.out.println("choose 2 for WITHDRAW");
        System.out.println("choose 3 for CHECK BALANCE");
        System.out.println("choose 4 for the EXIT FROM SYSTEM ");
        System.out.println("choose the operation you want to perform");
        int choice  = sc.nextInt();
        // USING SWITCH CASE TO MANAGE THE FUNCTIONS
        switch(choice){
            case 1 :
            System.out.println("enter the amount to deposite");
            int deposit = sc.nextInt();
            balance = balance + deposit; 
            System.out.println(" succesfull depsote the amount");
            System.out.println("the balance is: " + balance);
            System.out.println("");
            break;
            case 2 :
            System.out.println("enter the amount to widhdraw");
            int widhdraw = sc.nextInt();
            if(balance > widhdraw){
                balance = balance - widhdraw;
                System.out.println("collect the money");
                System.out.println("left balance:" + balance);
            }
            else{
                System.out.println("Insufficent balance");
            }
            System.out.println("");
            break ; 
            
            case 3: 
            System.out.println(" balance :" + balance);
            System.out.println("");
            break ; 
            case 4: 
            System.exit(0);


        }

        
    }
    
}
