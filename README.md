# RandomNumberGame
This is random number guessing game. A random number will be generated up to 100. The user will have to guess to the number. 


package random.number.game;
 import java.util.Random;//for random number generation
import java.util.Scanner;//for user input

public class RandomNumberGame {


    
     

 
    
    public static void main (String args[] ) 
 {
Random rand=new Random();//random number generation
int nguess=rand.nextInt(100);//random number can be generated up to 100
int ntries=0;//counter for finding number of tries
Scanner input =new Scanner(System.in);
int guess;
boolean bwin=false;
  
while(bwin==false)
{
System.out.println("Please guess a number :");
guess=input.nextInt();//user input his guess
ntries=ntries+1;//counter will increase by 1
if(guess==nguess)//if the guess is correct
{
bwin=true;
}
else if (guess < nguess)//if guessed number is less than actual number
{
System.out.println(+guess+ " is too low");
}
else if (guess > nguess)//if guessed number is greater than actual number
{
System.out.println(+guess+ " is too high");
}
}
  
System.out.println("Congratulation! You guessed the number in "+ntries + " guess(es)");
}
}
    
    

