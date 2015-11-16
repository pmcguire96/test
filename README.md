# test

import java.util.Scanner;
public class RockPaperScissors {
	
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		
		String user;
		System.out.print("Enter 'rock' 'paper' or 'scissors': ");
		user = sc.nextLine();
		
		String computer;
		double choice = 10 * Math.random();

		
		if (choice < 3.3333333)
		{
			computer = "rock";
		}
		else if (choice > 6.66)
		{
			computer = "paper";
		}
		else
		{
			computer = "scissors";
		}
		
		System.out.println("The computer chooses " + computer);
		
		if ((computer.equals("rock") && user.equals("scissors")) || (computer.equals("paper") && user.equals("rock") || (computer.equals("scissors") && user.equals("paper"))))
		{
			System.out.println(computer + " beats " + user + ".");
			System.out.println("You lose. The computers are taking over. Prepare for judgement day.");
		}
		
		else if ((computer.equals("rock") && user.equals("paper")) || (computer.equals("paper") && user.equals("scissors") || (computer.equals("scissors") && user.equals("rock"))))
		{
			System.out.println(user + " beats " + computer + ".");
			System.out.println("You win. We are safe. For now...");
		}
		
		else 
		{
			System.out.println("All chose " + user + ".");
			System.out.println("Tie. Practice more for next time.");
		}
	}
}
