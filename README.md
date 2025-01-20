# Day-14
Higher or Lower Game 🔼🔽
This is a Python-based "Higher or Lower" game, where players guess which account has more followers based on a given dataset.

Features
Account Comparisons:
Players are presented with two accounts, A and B, and must guess which one has a higher follower count.

Score Tracking:
The game keeps track of the player's score and displays it after each correct guess.

End Condition:
The game ends when the player makes an incorrect guess, and the final score is displayed.

How to Set Up
Ensure you have Python 3.x installed.

Save the code to a file, e.g., higher_or_lower.py.

Create the required art.py and game_data.py files:

art.py
Contains the ASCII art for the game. Example:
game_data.py
Contains the dataset with account information. Example:

python
Copy
Edit
data = [
    {"name": "Instagram", "follower_count": 3500, "description": "Social media platform", "country": "United States"},
    {"name": "Cristiano Ronaldo", "follower_count": 5500, "description": "Footballer", "country": "Portugal"},
    # Add more data as needed.
]
Run the program:

bash
Copy
Edit
python higher_or_lower.py  
How to Play
Start the Game:
Launch the program, and you'll be presented with two accounts, A and B.

Make Your Guess:
Type 'A' if you think account A has more followers, or 'B' if you think account B has more followers.

Check Your Answer:

If your guess is correct, your score increases, and the game continues.
If your guess is wrong, the game ends, and your final score is displayed.
Code Overview
Functions:

format_data(account): Formats account information into a readable string.
check_answer(user_guess, a_followers, b_followers): Checks if the player's guess is correct.
Gameplay Logic:

The game alternates accounts for comparisons and avoids comparing the same account against itself.
Player inputs are case-insensitive and validated for correctness.
Scoring:

The player's score increases by 1 for every correct guess.
The game ends when a guess is incorrect.
