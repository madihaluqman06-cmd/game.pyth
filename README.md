# game.pyth
import random

# Generate a random secret number between 1 and 100
secret_number = random.randint(1, 100)

print("🎯 Welcome to the Guessing Game!")
print("I have chosen a number between 1 and 100.")

while True:
    guess = int(input("Enter your guess: "))

    if guess < secret_number:
        print("Too Low! Try again.")
    elif guess > secret_number:
        print("Too High! Try again.")
    else:
        print("🎉 Congratulations! You guessed the correct number!")
        break
