# <p>**JAVA ASSIGNMENT**<p>
# <p>06 Switch Statement<p>
# <p>Let's Practice: Text-based Adventure<p>
## <p>**Interactive Exercise: Ultimate Adventure Game**<p>
## **Objective:**
### <p>In this exercise, you will create an Ultimate Adventure Game program in Java.<p>
## **Problem Statement:**
### <p>Create an adventure game in Java using only switch-case statements.<p>
### <p>1️. Present a welcome message and clearly state the player's objective.<p>
### <p>2️. Ask the player to make choices at each scenario.<p>
### <p>3️. Navigate through different scenarios based on choices.<p>
### <p>4️. Clearly handle invalid choices by displaying appropriate messages.<p>
### <p>5️. End the game when the player finds the treasure or encounters a trap.<p>
```
import java.util.Scanner;
public class AssignmentSix {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Welcome to the ultimate Adventure Game!");
        System.out.println("Your goal is to find the hidden treasure.Choose wisely");
        System.out.println("You are at a crossroad. Do you want to go left or right?");
        System.out.println("Type 'left' or 'right': ");
        String choice1 = sc.nextLine().toLowerCase();
        switch (choice1) {
            case "left":
                 System.out.println("You walk down a dark path and find a myserious cave.");
                 System.out.println("Do you want to enter the cave or walk past it? ");
                 System.out.println("Type 'enter' or 'walk' ");
                 String choice2 = sc.nextLine().toLowerCase();
                 switch (choice2){
                    case "enter":
                        System.out.println("Inside the case you will find a sleeping dragon!");
                        System.out.println("Do you want to fight the dragon of sneak past it? ");
                        System.out.println("Type 'fight' or 'sneak' ");
                        String choice3 = sc.nextLine().toLowerCase();
                        switch (choice3){
                            case "fight":
                                System.out.println("You bravely fight the dragon and the dragon impressed by your courage");
                                System.out.println("You are victorious! The dragon guards the treasure. You win!");
                                 break;
                            case "sneak":
                                 System.out.println("You sneak past the dragon and finds the treasure behind it. you win!");     
                            default:
                                System.out.println("Invalid choice. You got caught by the dragon and lost.");
                                break;
                        }
                        break;
                    case "walk":
                        System.out.println("You walk past the cave and fall into a hidden trap. Game over");
                        break;
                    default:
                        System.out.println("Invalid choice. You lost the Game! ");
                        break;

                    }
        break;
            case "right":
                 System.out.println("You walk through a dense forest and find a river.");
                 System.out.println("Do you want to swim across or build a raft?");
                 System.out.println("Type 'swim' or 'raft' ");
                 String choice2b = sc.nextLine();
                 switch (choice2b){
                    case "swim":
                        System.out.println("You swim across the river and encounter a wild bear!");
                        System.out.println("Do you want to run away or climb a tree? ");
                        System.out.println("Type 'run' or 'climb': ");
                        String choice3b = sc.nextLine();
                        switch (choice3b){
                            case "run":
                                System.out.println("You run away safely and find a hidden path to the treasure. You win!");
                                break;
                            case "climb":
                                System.out.println("You climb the tree, but the bear waits for you. You are stuck. Gme over.");    
                                break;
                            default:
                                System.out.println("Invalid choice. The bear catches you. Game over.");        
                        }
                        break;
                    case "raft":
                        System.out.println("You build a raft and safely cross the river. You find the treasure on the other side. You win!");
                        break;
                    default:
                        System.out.println("Invalid choice. You got swept away by the river. Game over.");
                        break;
                    }
        break;
         default:
            System.out.println("Invalid choice. You got lost in the wilderness. Game over.");
            break;
           
            }
                 
             sc.close();  

        }           
    }
```
[githublink](https://github.com/Aromalpriyan/Assignment---6)