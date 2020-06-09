# Summary
This program randomly picks a number from 1 to 100. The user is then asked to guess a number between 1 to 100. If the user picks a wrong number it will then tell the user that their number is either too high or too low. The program also keep count of how many tries it took the user to guess the correct number. When the user guesses the correct number a message will apear congratulating the User. 
## public class RandomNumberGame

### Random number generator. 
Random rand=new Random();//random number generation

#### ints
int nguess=rand.nextInt(100);//random number can be generated up to 100
int ntries=0;//counter for finding number of tries
int guess;

##### booleans
boolean bwin=false;
bwin=true

###### while,if, else if 
while(bwin==false)
if(guess==nguess)//if the guess is correct
else if (guess < nguess)//if guessed number is less than actual number
else if (guess > nguess)//if guessed number is greater than actual number
