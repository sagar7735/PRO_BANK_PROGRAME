
import java.util.Scanner;

class Bank{
private double bal=10000;
private int pwd;
public void deposite(double money){
	System.out.println("ENTER PASSWORD");
	Scanner s=new Scanner(System.in);
	pwd=s.nextInt();
	if(pwd==7735) {
		bal=bal+money;
		System.out.println("Deposited money :"+money);
		System.out.println("total Balance :"+bal);
	}
	else {
		System.out.println("YOU ENTERD PASSWORD");
	}
}
public void withdraw(double money) {
	System.out.println("ENTER PASSWORD");	
	Scanner s=new Scanner(System.in);
	pwd=s.nextInt();
	if(pwd==7735) {
		bal=bal-money;
		System.out.println("WITHDRAW MONEY :"+money);
	   System.out.println("TOTAL BALANCE :"+bal);
	}
	else {
		System.out.println("YOU ENTER INVALID PASSWORD");
	}
}
public void checkbal() {
System.out.println("ENTER PASSWORD");
Scanner s=new Scanner(System.in);
pwd=s.nextInt();
if(pwd==7735) {
	System.out.println("TOTAL BALANCE :"+bal);
}
/*else {
	System.out.println("INVALID PASSWORD");
}*/
}
}
public class PRO_BANK_PROGRAME {

	public void main(String []args) {
		// TODO Auto-generated method stub
Bank b=new Bank();
int ch;
System.out.println(" 1. DEPOSITE :");
System.out.println(" 2. WITHDRAW :");
System.out.println(" 3. CHECKBALANCE :");

 System.out.println("enter your choice");
 Scanner s2=new  Scanner(System.in);
 ch=s2.nextInt();
 
 switch(ch) {
 case 1: b.deposite(1000);
 break;
 case 2: b.withdraw(500);
 break;
 case 3: b.checkbal();
 break;
 default: System.out.println("invalid choice");
 
 }
	
	
	}

}


