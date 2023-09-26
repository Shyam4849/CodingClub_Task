# CodingClub_Task
This is my first task 
<br>
My task is to create Rock, Paper, Scissor game.
<br>

import java.util.Scanner;
import java.util.Random;
public class RockPaperScissor {
    public static void main(String[] args) {
        System.out.println("Lets start the game");
        Scanner sc =  new Scanner (System.in);
        System.out.println("1 for Rock");
        System.out.println("2 for Paper");
        System.out.println("3 for  Scissor");
        System.out.println("Please select a number");
        int num = sc.nextInt();

        System.out.println("You selected: ");
        switch(num){
            case 1 -> System.out.println("Rock");
            case 2 -> System.out.println("Paper");
            case 3 -> System.out.println("Scissor");
        }

        Random random = new Random();
        int number = random.nextInt(1,3);

        System.out.println("The computer selected: ");
        switch(number){
            case 1 -> System.out.println("Rock");
            case 2 -> System.out.println("Paper");
            case 3 -> System.out.println("Scissor");
        }

        if (number == num) {
            System.out.println("Draw");
        }
        else if (num == 1 && number == 2){
            System.out.println("Computer wins");
        }
        else if (num == 1 && number == 3){
            System.out.println("You win");
        }
        else if (num == 2 && number == 1){
            System.out.println("You win");
        }
        else if (num == 2 && number == 3){
            System.out.println("Computer wins");
        }
        else if (num == 3 && number == 1){
            System.out.println("Computer wins");
        }
        else if (num == 3 && number  == 2){
            System.out.println("You win");
        }

    }
}
