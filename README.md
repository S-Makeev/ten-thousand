# Lab - Class 06

## Project: ten-thousand

Author: Sarah Glass, Logan Reese, and Slava Makeev for Python 401

## Overview

Create a command line version of the dice game Ten Thousand.

Today is all about tackling the highest risk and/or highest priority features - scoring and dice rolling.

- Define a GameLogic class in ten_thousand/game_logic.py file.

- Handle calculating score for dice roll

- Add calculate_score static method to GameLogic class.

- The input to calculate_score is a tuple of integers that represent a dice roll.

- The output from calculate_score is an integer representing the roll’s score according to rules of game.


**Handle rolling dice**

- Add roll_dice static method to GameLogic class.

- The input to roll_dice is an integer between 1 and 6.

- The output of roll_dice is a tuple with random values between 1 and 6.

- The length of tuple must match the argument given to roll_dice method.

- Using the parameters above, use ChatGPT to generate code blocks.

- You must document every single line of code with a detailed description of what the code is doing.

## Links and Resources

- Lots of TA and peer help.
- Referenced class demo
- Chat GPT - prompts and output are documented in the "chatgpt.md" file

## Setup

No .env requirements; gitignore invludes venv.

## How to initialize/run your application

- python3 game_logic.py
- python3 test_ten_thousand.py

## How to use your library

No external libraries were brought in.

## Tests

All acceptance testing run through test_series.py file and pytest following TDD.

--------------------------------------------

# Lab - Class 07

## Project: ten-thousand

Author: Sarah Glass, Logan Reese, and Slava Makeev for Python 401

## Overview

Create a command line version of the dice game Ten Thousand.

Extend Ten Thousand game started in previous class to get the game in playable state.

Application should implement all features from previous version
Application should allow user to set aside dice each roll
Application should allow “banking” current score or rolling again.
Application should keep track of total score
Application should keep track of current round


## Links and Resources

- Lots of TA and peer help.
- Referenced class demo
- Chat GPT - prompts and output are documented in the "chatgpt.md" file

## Setup

No .env requirements; gitignore invludes venv.

## How to initialize/run your application

- python3 game_logic.py
- python3 game.py

## How to use your library

The library we brought in is flo.py

## Tests

All acceptance testing run through test_series.py file and pytest following TDD.


-----------------------------------------------

# Lab - Class 08

## Project: ten-thousand

Author: Sarah Glass, Logan Reese, and Slava Makeev for Python 401

## Overview

Create a command line version of the dice game Ten Thousand.

Let’s shore up the core functionality of game by allowing users to set aside scoring dice and continuing their turn.

Then we’ll handle cheaters and/or confused players who are skirting the rules.

-Application should implement features from versions 1 and 2
-Should handle setting aside scoring dice and continuing turn with remaining dice.
-Should handle when cheating occurs.
Or just typos.
E.g. roll = [1,3,5,2] and user selects 1, 1, 1, 1, 1, 1
-Should allow user to continue rolling with 6 new dice when all dice have scored in current turn.
-Handle zilch
-No points for round, and round is over
-Accounts for proper banking 
-Implemented zilch functionality if the last roll doesn't score points. 

## Links and Resources

- Lots of TA and peer help.
- Referenced class demo
- Chat GPT - prompts and output are documented in the "chatgpt.md" file

## Setup

No .env requirements; gitignore invludes venv.

## How to initialize/run your application

- python3 ten_thousand.game

## How to use your library

The library we brought in is flo.py

## Tests

We are working our way through testing. Console will bank and carry over points, but currenlty won't accept more than one die's points at a time.
