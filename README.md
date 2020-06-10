# Summary
This program randomly picks a number from 1 to 100. The user is then asked to guess a number between 1 to 100. If the user picks a wrong number it will then tell the user that their number is either too high or too low. The program also keep count of how many tries it took the user to guess the correct number. When the user guesses the correct number a message will apear congratulating the User. This program only has one class.
# Random Int
Random rand=new Random();//random number generation
int nguess=rand.nextInt(100);//random number can be generated up to 100
int ntries=0;//counter for finding number of tries

## Scanner
Scanner input =new Scanner(System.in); // scans for user input
int guess;
boolean bwin=false; // sets boolean bwin equal to false
  
while(bwin==false) // while boolean bwin is equal to false

### UserInput

guess=input.nextInt();//user input their guess
ntries=ntries+1;//counter will increase by 1
if(guess==nguess)//if the guess is correct
{
bwin=true;
}
else if (guess < nguess)//if guessed number is less than actual number

#### SystemOutput
System.out.println("Please guess a number :"); // displays the message "Please guess a number".
System.out.println(+guess+ " is too low"); //displays the message 
system.out.println(+guess+ " is too high");//displays the message
System.out.println("Congratulation! You guessed the number in "+ntries + " guess(es)"); //displays the message


