# Rock-Paper-scissor-Game.py
I have made this rock paper scissor game to make my understanding better in statements 
import random

user_choice = int(input("Enter your choice:\nType 0 For Rock\nType 1 For Paper\nType 2 For Scissor\n"))

if user_choice >= 3 or user_choice < 0:
    print("You entered invalid number, You dumbass.")
    
else:
    computer_choice = random.randint(0, 2)
    print(f"Computer Chose: {computer_choice}")
    
    if user_choice == computer_choice:
        print("It's a draw")
    elif (user_choice == 0 and computer_choice == 2) or \
         (user_choice == 1 and computer_choice == 0) or \
         (user_choice == 2 and computer_choice == 1):
        print("You Win")
    else:
        print("You Lose")
