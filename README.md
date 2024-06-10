# Guess The Number

The Guesse The Number Game is a simple Python program that allows users to guess a randomly generated number or have the computer guess their number. 

## Installation Instructions

1. Clone the repository:

    ```
    git clone https://github.com/Rafsun07/Guess-The-Number.git
    cd guess-the-number
    ```

2. Run the game:

    ```
    python guess-the-number.py
    ```

## Usage

1. **Start the game:**

    Run the `guess-the-number(user).py` or `guess-the-number(computer).py` script to start the Guessing game.

2. Computer:
   
   You will be prompted to guess a randomly generated number between the specified range. Enter your guess when prompted and the program will provide feedback on whether your guess is too high, too low, or correct.

3. USer:

   This time, the computer will prompt you to think of a number within the specified range. Once you have chosen a number, follow the prompts to inform the computer whether its guesses are too high, too low, or correct. The computer will continue guessing until it correctly identifies your number.

## How the Code Works

### guess(x) Function:

- This function takes an argument x, which represents the upper limit of the range within which the random number will be chosen.
- It generates a random number between 1 and x (inclusive) using random.randint(1, x).
- It enters a loop where the user is prompted to guess the number.
- Inside the loop:
     - The user input is converted to an integer and stored in the variable guess.
     - If the guess is lower than the random number, it informs the user that their guess is too low.
     - If the guess is higher than the random number, it informs the user that their guess is too high.
- The loop continues until the user's guess matches the random number.
- Once the guess matches the random number, it congratulates the user and reveals the correct number.

### computer_guess(x) Function:

- This function also takes an argument x, representing the upper limit of the range within which the user's number will be.
- It initializes low as 1 and high as x, representing the range of possible numbers.
- It enters a loop where the computer makes guesses.
- Inside the loop:
     - It generates a guess using random.randint(low, high).
     - The user provides feedback on whether the guess is too high, too low, or correct.
     - Depending on the feedback:
        - If the guess is too high, it adjusts the high value to be one less than the guess.
        - If the guess is too low, it adjusts the low value to be one more than the guess.
        - If the guess is correct, the loop exits.
- Once the loop exits, it congratulates the computer and reveals the correct guess.
  
Both functions provide an interactive way to play a number guessing game, one where the user tries to guess the computer's number and the other where the computer tries to guess the user's number.


## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes. Ensure that your code follows the project's coding standards and includes appropriate tests.

## Contact

For questions, suggestions, or issues, please open an issue on GitHub or contact the project maintainer at [rafsun.eram@gmail.com](mailto:rafsun.eram@gmail.com).

## Acknowledgements

- Developed using Python.
- Inspired by classic game of Guessing Numbers.

---


   
