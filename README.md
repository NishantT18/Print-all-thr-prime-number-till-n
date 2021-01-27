# Print-all-the-prime-number-till-n

import java.util.*;
public class Main
{
	public static void main(String[] args) {
		//System.out.println("Hello World");
		Scanner scn = new Scanner(System.in);
		int n = scn.nextInt();
		printprime(n);
	}
	
	public static boolean IsPrime(int n){
	    if(n <= 1){
	        return false;
	    }
	    for(int i = 2; i < n; i++){
	        if(n%i==0){
	            return false;
	        }
	        
	    }
	    return true;
	}
	public static void printprime(int n){
	    for (int i = 2; i <= n; i++){ 
            if (IsPrime(i)){ 
                System.out.print(i + " "); 
            } 
	    }
    }
}

