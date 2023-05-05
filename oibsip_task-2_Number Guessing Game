import java.util.Scanner;
import java.util.Random;
class Game
{
//sI=system input and uI=user input
int sI;
int uI;
int noOfGuesses=0;
Game()
{
Random random=new Random();
this.sI=random.nextInt(100) + 1;
}
public boolean takeUserInput()
{
if(noOfGuesses<10)
{
System.out.println("Guess the number : ");
this.uI=GuessTheNumber.takeIntegerInput(100);
noOfGuesses++;
return false;
}
else
{
System.out.println("Number of attempts finished...Better luck next time\n");
return true;
}
}
public boolean isCorrectGuess()
{
if(sI==uI)
{
System.out.println("Congratulations, you guess the number " + sI +  "  in  " +  noOfGuesses + " guesses ");
switch(noOfGuesses)
{
case 1:
System.out.println("Your Score is 100");
break;
case 2:
System.out.println("Your Score is 90");
break;
case 3:
System.out.println("Your Score is 80");
break;
case 4:
System.out.println("Your Score is 70");
break;
case 5:
System.out.println("Your Score is 60");
break;
case 6:
System.out.println("Your Score is 50");
break;
case 7:
System.out.println("Your Score is 40");
break;
case 8:
System.out.println("Your Score is 30");
break;
case 9:
System.out.println("Your Score is 20");
break;
case 10:
System.out.println("Your Score is 10");
break;
}
System.out.println();
return true;
}
else if(noOfGuesses<10 && uI>sI)
{
if(uI-sI >10)
{
System.out.println("Too High");
}
else
{
System.out.println("Little High");
}
}
else if(noOfGuesses<10 && uI<sI)
{
if(sI-uI>10)
{
System.out.println("Too Low");
}
else
{
System.out.println("Little Low");
}
}
return false;
}
}
class GuessTheNumber
{
public static int takeIntegerInput(int limit)
{
int input=0;
boolean flag=false;
while(!flag)
{
try
{
Scanner sc=new Scanner(System.in);
input=sc.nextInt();
flag=true;
if(flag && input > limit || input<1)
{
System.out.println("choose the number between 1 to "+limit);
flag=false;
}
}
catch(Exception e)
{
System.out.println("Enter only integer values");
flag=false;
}
};
return input;
}
public static void main(String args[])
{
System.out.println("1. Start the Game\n2. Exit");
System.out.println("Enter your choice : ");
System.out.println("cdcd1. Start the Game : ");
System.out.println("Enter your choice : ");
int choice=takeIntegerInput(2);
int nextRound=1;
int noOfRound=0;
if(choice==1)
{
while(nextRound==1)
{
Game game=new Game();
boolean isMatched=false;
boolean isLimitCross=false;
System.out.println("\nRound "+ ++noOfRound +"starts...");
while(!isMatched && !isLimitCross)
{
isLimitCross=game.takeUserInput();
isMatched=game.isCorrectGuess();
}
System.out.println("1.Next Round \n2. Exit");
System.out.println("Enter your choice : ");
nextRound=takeIntegerInput(2);
if(nextRound !=1)
{
System.exit(0);
}
}
}
else
{
System.exit(0);
}
}
}
  

