# Number-Guessing-Game
# Simple number guessing game

secret_number = 7
guess_count = 0
max_guesses = 3

while guess_count < max_guesses:
    guess = int(input("Guess a number between 1 and 10 : "))
    guess_count += 1

    if guess == secret_number:
        print("Congratulation! You guessed the correct number! ")
        break
    elif guess < secret_number:
        print("Too Low!")
    else:
        print("Too High!")
    # Tell the user how many guesses they have left.

    guesses_left = max_guesses - guess_count
    if guesses_left > 0:
        print(f"You have {guesses_left} guesses left.")
else:
    print(f"Sorry, you've used all the {max_guesses} guesses. The secret number was {secret_number}. ")
