# Python-Task
Creating and using local python packages

import random

while True:
    choices = ["R","P","S"]

    computer = random.choice(choices)
    player = None 
    
    while player not in choices:
        print("Error, input again")
        player = input("Pick an option between R, P, or S?: ").upper()

    print("computer: ",computer)
    print("player: ",player)

    if player == computer:
        print("computer: ",computer)
        print("player: ",player)
        print("Tie")
    elif player == "R":
        if computer == "P":
            print("computer: ",computer)
            print("player: ",player)
            print("You lose!")
        if computer == "S":
            print("computer: ",computer)
            print("player: ",player)
            print("You win!")
    elif player == "S":
        if computer == "R":
            print("computer: ",computer)
            print("player: ",player)
            print("You lose!") 
        if computer == "P":
            print("computer: ",computer)
            print("player: ",player)
            print("You win!")
    elif player == "P":
        if computer == "S":
            print("computer: ",computer)
            print("player: ",player)
            print("You lose!")
        if computer == "R":
            print("computer: ",computer)
            print("player: ",player)
            print("You win!")

    play_again = input("Play again? (yes/no): ").lower()

    if play_again !="yes":
        break

print("Goodbye!!")
