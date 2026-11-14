# python-number-guessing-game
# A beginner Python game where the player guesses a randomly chosen number from 1 to 10.

import random
secret_number = random.randint(1, 10)
while True:
    guess = int(input("Guess a number from 1 to 10: "))

    if guess == secret_number:
        print("You got it!")
        break
    elif guess < secret_number:
        print("Too low. Try again.")
    else:
        print("Too high. Try again.")
