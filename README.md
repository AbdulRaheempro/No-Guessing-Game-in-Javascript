# No-Guessing-Game-in-Javascript
A console-based JavaScript game where players guess two numbers to win a prize. It offers multiple chances to guess correctly, providing feedback and instructions based on the player's inputs.
Title: Number Guessing Game

Description: This console-based game challenges the user to enter a specific sequence of numbers to win a prize. The user has multiple chances to input the numbers correctly, with different messages and outcomes depending on the trial and correctness of the inputs.

Key Features
Multiple Trials: The game allows the user several chances to input the correct numbers:

First Trial: The user enters two numbers and receives feedback based on their correctness.
Second Trial: If the first input is incorrect, the user has a chance to correct the second number.
Last Chance: If the second trial is also unsuccessful, the user is given one final chance.
Winning Conditions:

First Trial Win: Correctly inputting both numbers (33 and 43) on the first attempt wins the game.
Second Trial Win: Correctly inputting the second number (43) after the first number is incorrect wins the game.
Third Trial Win: Correctly inputting the first number (33) after failing the first trial wins the game.
Feedback Messages: The game provides different messages based on user inputs and the result of each trial:

Success messages with prize announcements.
Error messages with encouragement for better luck next time.
Detailed Functions
end() Function:

Provides a final chance for the user to enter a number and checks if it matches either 33 or 43.
Displays a win or loss message based on the input.
lastchance2() Function:

Asks for the final input and checks if it matches 33.
Provides congratulatory or losing messages based on the input.
onetimeinput() Function:

Handles the final input for when the user fails the previous trials.
Checks if the input matches 43 and provides appropriate feedback.
input2nd() Function:

Checks if the second number input matches 43.
Provides a congratulatory message for a win or proceeds to the onetimeinput() function if the input is incorrect.
input1st() Function:

Checks if the first number input matches 33.
Provides a congratulatory message for a win or proceeds to the lastchance2() function if the input is incorrect.
userinput() Function:

Handles the initial input of two numbers.
Determines the next steps based on the correctness of the inputs, calling other functions as needed.
Recursively calls itself if both numbers are incorrect, providing multiple chances for the user.
Code Analysis
Loop Usage: In your code, the for loops with i <= 1 are unnecessary because the logic is designed to handle single inputs at each stage. You can remove these loops to simplify the code.

Error Handling: Ensure correct case for logging messages (e.g., console.log instead of CONSOLE.LOG).

Logical Conditions: The condition if(t==33 &&t==43) in the end() function is never true because a single value cannot be equal to both 33 and 43. This should be corrected to check for either value
