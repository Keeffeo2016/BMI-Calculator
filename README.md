# BMI-Calculator
Java BMI Calculator


import java.util.Scanner;
public class BMI {
	
	double bmi;
	
	static void blurb(){
		System.out.printf("Welcome to James BMI Calculator,Where its nice to see mee to see me its nice!!!. ");
		System.out.println("\n--------------------------------------------------------------------------------");
	    
		Scanner input = new Scanner(System.in);
	     
	     System.out.print("Enter your weight in Kilograms: ");
	     double weightInKilogram = input.nextDouble();
	         
	     System.out.print("Enter your height in Meters: ");
	     double heightInMeters = input.nextDouble();
	     
	     double bmi = weightInKilogram / (heightInMeters * heightInMeters);// BMI Calculated
	     System.out.printf("Your Body Mass Index is %.2f " , bmi);
	     
	}
	     
	     
	     
		void BMIValues (){    
	     
	    if (bmi < 18.5)
	       System.out.println("You are seriously underweight");
	     else if (bmi <=18.6 && bmi >= 24.9)
	       System.out.println("You are normal weight");
	     else if (bmi <= 25 && bmi >= 29.9)
	       System.out.println("You are overweight");
	     else if (bmi <30)
	       System.out.println("You are Obese");
		}
	     
	    
	    
  public static void main(String[] args) {
	    BMI app = new BMI();
	    app.blurb();
	    app.BMIValues();
	    	
  }//end Main
	
}//End Class
	     
	     

	


