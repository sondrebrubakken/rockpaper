# rockpaper
rock paper


import random

while True:
    choice = ["rock", "paper", "scissors"]

    computer = random.choices(choice)
    player = None

    while player not in choice:
        player = input("rock, paper, scissors?").lower()
        
    if player == computer:
        print (f"computer: {computer} ")
        print (f"player: {player}")
        print ("Tie!")

    elif player == "rock":
        if computer == "scissors":
            print(f"computer: {computer}")
            print(f"player: {player}")
            print("You win!")
        if computer == "paper":
            print(f"computer: {computer}")
            print(f"player: {player}")
            print("You lose!")

    elif player == "scissors":
        if computer == "rock":
            print(f"computer: {computer}")
            print(f"player: {player}")
            print("You Lose!")
        if computer == "paper":
            print(f"computer: {computer}")
            print(f"player: {player}")
            print("You Win!")
            
    elif player == "paper":
        if computer == "rock":
            print(f"computer: {computer}")
            print(f"player: {player}")
            print("You Win!")
        if computer == "scissors":
            print(f"computer: {computer}")
            print(f"player: {player}")
            print("You lose!")


    replay = input("Rematch? (yes/no): ").lower
    if replay != "yes":
        break




