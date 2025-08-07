import random

print("🎯 Welcome to the Number Guessing Game!")
print("I'm thinking of a number between 1 and 100.")

number_to_guess = random.randint(1, 100)
attempts = 0

while True:
    guess = int(input("Enter your guess: "))
    attempts += 1

    if guess < number_to_guess:
        print("📉 Too low! Try again.")
    elif guess > number_to_guess:
        print("📈 Too high! Try again.")
    else:
        print(f"✅ Correct! You guessed the number in {attempts} attempts.")
        break
