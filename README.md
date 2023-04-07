# Display_-sbn
This program calculates the last digit of isbn number


import java.util.Scanner;

//Kadir PEKDEMİR 


public class DisplaysIsbn {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		
		//Create Scanner
		Scanner input = new Scanner(System.in);
		System.out.print("Enter the first 9 digits of an ISBN as integer:");
		int isbn9 = input.nextInt();
		
		//Calculate last digit based on number of digits
		int lastStep1 = ((int)(isbn9/Math.pow(10,8))*1+(int)((isbn9%Math.pow(10,8))/Math.pow(10,7))*2+(int)((isbn9%Math.pow(10,7))/Math.pow(10,6))*3+(int)((isbn9%Math.pow(10,6))/Math.pow(10,5))*4+(int)((isbn9%Math.pow(10,5))/Math.pow(10,4))*5+(int)((isbn9%Math.pow(10,4))/Math.pow(10,3))*6+(int)((isbn9%Math.pow(10,3))/Math.pow(10,2))*7+(int)((isbn9%Math.pow(10,2))/Math.pow(10,1))*8+(int)((isbn9%Math.pow(10,1))/Math.pow(10,0))*9)%11;
		int lastStep2 = ((int)(isbn9/Math.pow(10,7))*2+(int)((isbn9%Math.pow(10,7))/Math.pow(10,6))*3+(int)((isbn9%Math.pow(10,6))/Math.pow(10,5))*4+(int)((isbn9%Math.pow(10,5))/Math.pow(10,4))*5+(int)((isbn9%Math.pow(10,4))/Math.pow(10,3))*6+(int)((isbn9%Math.pow(10,3))/Math.pow(10,2))*7+(int)((isbn9%Math.pow(10,2))/Math.pow(10,1))*8+(int)((isbn9%Math.pow(10,1))/Math.pow(10,0))*9)%11;
		int lastStep3 = ((int)(isbn9/Math.pow(10,6))*3+(int)((isbn9%Math.pow(10,6))/Math.pow(10,5))*4+(int)((isbn9%Math.pow(10,5))/Math.pow(10,4))*5+(int)((isbn9%Math.pow(10,4))/Math.pow(10,3))*6+(int)((isbn9%Math.pow(10,3))/Math.pow(10,2))*7+(int)((isbn9%Math.pow(10,2))/Math.pow(10,1))*8+(int)((isbn9%Math.pow(10,1))/Math.pow(10,0))*9)%11;
		int lastStep4 = ((int)(isbn9/Math.pow(10,5))*4+(int)((isbn9%Math.pow(10,5))/Math.pow(10,4))*5+(int)((isbn9%Math.pow(10,4))/Math.pow(10,3))*6+(int)((isbn9%Math.pow(10,3))/Math.pow(10,2))*7+(int)((isbn9%Math.pow(10,2))/Math.pow(10,1))*8+(int)((isbn9%Math.pow(10,1))/Math.pow(10,0))*9)%11;
		int lastStep5 = ((int)(isbn9/Math.pow(10,4))*5+(int)((isbn9%Math.pow(10,4))/Math.pow(10,3))*6+(int)((isbn9%Math.pow(10,3))/Math.pow(10,2))*7+(int)((isbn9%Math.pow(10,2))/Math.pow(10,1))*8+(int)((isbn9%Math.pow(10,1))/Math.pow(10,0))*9)%11;
		int lastStep6 = ((int)(isbn9/Math.pow(10,3))*6+(int)((isbn9%Math.pow(10,3))/Math.pow(10,2))*7+(int)((isbn9%Math.pow(10,2))/Math.pow(10,1))*8+(int)((isbn9%Math.pow(10,1))/Math.pow(10,0))*9)%11;
		int lastStep7 = ((int)(isbn9/Math.pow(10,2))*7+(int)((isbn9%Math.pow(10,2))/Math.pow(10,1))*8+(int)((isbn9%Math.pow(10,1))/Math.pow(10,0))*9)%11;
		int lastStep8 = ((int)(isbn9/Math.pow(10,1))*8+(int)((isbn9%Math.pow(10,1))/Math.pow(10,0))*9)%11;
		int lastStep9 = ((int)(isbn9/Math.pow(10,0))*9)%11;
		
		
		//Print by different digit numbers
		if ((int)((isbn9/Math.pow(10,8))) >= 1)
 
			//If the result of the last digit is x10, write x
			if (lastStep1 == 10)
				System.out.println("The ISBN-10 number is " + isbn9+""+"X");
			else
				System.out.println("The ISBN-10 number is " + isbn9+""+lastStep1);
		
		else if  ((int)((isbn9/Math.pow(10,7))) >= 1)
			
			//If the result of the last digit is x10, write x
			if (lastStep2 == 10)
				System.out.println("The ISBN-10 number is " +"0"+""+isbn9+""+"X");
			else
				System.out.println("The ISBN-10 number is " +"0"+""+isbn9+""+lastStep2);
		
		else if  ((int)((isbn9/Math.pow(10,6))) >= 1)
			
			//If the result of the last digit is x10, write x
			if (lastStep3 == 10)
				System.out.println("The ISBN-10 number is " +"00"+""+isbn9+""+"X");
			else
				System.out.println("The ISBN-10 number is " +"00"+""+isbn9+""+lastStep2);
		
		else if  ((int)((isbn9/Math.pow(10,5))) >= 1)
			
			//If the result of the last digit is x10, write x
			if (lastStep4 == 10)
				System.out.println("The ISBN-10 number is " +"000"+""+isbn9+""+"X");
			else
				System.out.println("The ISBN-10 number is " +"000"+""+isbn9+""+lastStep2);
		
		else if  ((int)((isbn9/Math.pow(10,4))) >= 1)
			
			//If the result of the last digit is x10, write x
			if (lastStep5 == 10)
				System.out.println("The ISBN-10 number is " +"0000"+""+isbn9+""+"X");
			else
				System.out.println("The ISBN-10 number is " +"0000"+""+isbn9+""+lastStep2);
		
		else if  ((int)((isbn9/Math.pow(10,3))) >= 1)
			
			//If the result of the last digit is x10, write x
			if (lastStep6 == 10)
				System.out.println("The ISBN-10 number is " +"00000"+""+isbn9+""+"X");
			else
				System.out.println("The ISBN-10 number is " +"00000"+""+isbn9+""+lastStep2);
		
		else if  ((int)((isbn9/Math.pow(10,2))) >= 1)
			
			//If the result of the last digit is x10, write x
			if (lastStep7 == 10)
				System.out.println("The ISBN-10 number is " +"000000"+""+isbn9+""+"X");
			else
				System.out.println("The ISBN-10 number is " +"000000"+""+isbn9+""+lastStep2);
		
		else if  ((int)((isbn9/Math.pow(10,1))) >= 1)
			
			//If the result of the last digit is x10, write x
			if (lastStep8 == 10)
				System.out.println("The ISBN-10 number is " +"0000000"+""+isbn9+""+"X");
			else
				System.out.println("The ISBN-10 number is " +"0000000"+""+isbn9+""+lastStep2);
		
		else if  ((int)((isbn9/Math.pow(10,0))) >= 1)
			
			//If the result of the last digit is x10, write x
			if (lastStep9 == 10)
				System.out.println("The ISBN-10 number is " +"00000000"+""+isbn9+""+"X");
			else
				System.out.println("The ISBN-10 number is " +"00000000"+""+isbn9+""+lastStep2);
		
				
			
	}

}
