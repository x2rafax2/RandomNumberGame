# Summary
This program randomly picks a number from 1 to 100. The user is then asked to guess a number between 1 to 100. If the user picks a wrong number it will then tell the user that their number is either too high or too low. The program also keep count of how many tries it took the user to guess the correct number. When the user guesses the correct number a message will apear congratulating the User. This program only has one class.
# Random Int
Random rand=new Random();//random number generation
int nguess=rand.nextInt(100);//random number can be generated up to 100
int ntries=0;//counter for finding number of tries

## Scanner
Scanner input =new Scanner(System.in);
int guess;
boolean bwin=false;
  
while(bwin==false)

### UserInput
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



