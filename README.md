package studio2;

import java.util.Scanner;

public class Ruin {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
    Scanner in = new Scanner(System.in);
    
    System.out.println("StartAmount");
    double StartAmount = in.nextDouble();
    System.out.println("winChance");
    
    double winChance = in.nextDouble();
    System.out.println("winLimit");
    double winLimit = in.nextDouble();
    System.out.println("total simulations");
    
    System.out.println("totalS");
    
    int totalS = in.nextInt();
    
    for (int dayNumber = 1; dayNumber < totalS; dayNumber ++)
    {
    	System.out.println(dayNumber);
    	while (StartAmount > 0 && StartAmount < winLimit) {
    		double x = Math.random();
    		if( x <= winChance ) {
    	    StartAmount++;}
    		else {
        	StartAmount--; }
    }
    }
    
    
    
    
    
		
		
	}

}
