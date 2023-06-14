# Final-project-on-numer-game
COGS 18 Fianl project on guessing the number game
import random

# Generate a random number between 1 and 1000
number = random.randint(1, 1000)

# Keep track of the number of guesses
num_guesses = 0

# Loop until the user guesses the correct number
while True:
    # Ask the user for a guess
    guess = int(input("Guess a number between 1 and 1000: "))
    
    # Increment the number of guesses
    num_guesses += 1
    
    # Check if the guess is correct and provide feedback
    if guess == number:
        print("Finally Dude, you guessed the number in {num_guesses} guesses! Ok, You went above average!")
    elif guess < number:
        print("Too low, just give up.")
    else:
        print("Too high, do better.")
