import random

# 🎲 Generate a random number between 1 and 100
target_number = random.randint(1, 100)
guess_count = 0

print("Welcome to the Number Guessing Game!")
print("I'm thinking of a number between 1 and 100. Can you guess it?")

while True:
    guess = int(input("Enter your guess: "))
    guess_count += 1

    if guess > target_number:
        print("Lower number please.")
    elif guess < target_number:
        print("Higher number please.")
    else:
        print(f"🎉 Congratulations! You guessed the number in {guess_count} tries.")
        break


