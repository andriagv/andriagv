//tite-GIVE ME A FIVE

/*So they invented a game to crush numbers to pieces. 
Since they were five, student i (for i=0,…,4) took care of 
numbers n where n%5 == i (here, % is the modulo operator in Java),
 i.e., when the rest of n after division by 5 is i.

0-divide by 5
1-add 9
2-subtract 1
3-add 7
4-add 6

Their old math teacher saw these rules and laughed at them: 
What? in most cases, the number is only increased!
You will never crush large numbers to 1 in this way!
Is this teacher right? Implement the game of the five students in MiniJava.
Your program should ask a number from the math teacher.
Then it should iteratively apply the student rules until the number is crushed,
 i.e., reduces to a value ≤1\leq 1≤1. Once this has occurred, 
 it should return the number of iterations that have been performed.
*/

import java.util.Scanner;

public class Main {

	public static void main(String[] args) {
	
		Scanner keyboard = new Scanner(System.in);
        
        int y = 0;
        int x = keyboard.nextInt();
          System.out.println("your choosen number is : " +x);
          System.out.println("received numbers: ");
		  while (x>1) { 
           if(x%5==0){x=x/5;
                      }                                                                                                
              else if(x%5==1){
                 x=x+9;   }
              else if(x%5==2){
                 x=x-1;   }
              else if(x%5==3){
            	  x=x+7;  }
              else if (x%5==4){
                 x=x+6;   }
                 
                 System.out.println(x);             
                 y=y+1; 
                                }
		    System.out.println("number of actions: "+ y);
	        keyboard.close();

	    }  
    }  //inst of the autor: andria.gv
