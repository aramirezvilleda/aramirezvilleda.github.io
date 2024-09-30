```mermaid

graph TD;
	A([Start])  ----> B([Computer chooses number between 1-100]);
    B ----> C([Computer instructs: **_Choose a number between 1-100_**]);
    C -- The player inserts their number --> D([Computer compares the numbers]);
    D ----> E([Do they match?]);

    E -- Yes --> F([Computer Displays: **_CORRECT_**!]);
    F ----> G([Computer asks: **_TRY AGAIN?_**]);
    G -- Yes --> B;
    G -- No --> H([End]);

    E -- No --> I([Is the player's number higher than the computers'?]);
    I -- Yes --> J([Computer instructs: **_GUESS LOWER!_**]);
    J ----> C;
    I -- No --> K([Computer instructs: **_GUESS HIGHER!_**]);
    K ----> C;

```

The first batch of lines lay out the general process that will happen when the game starts. The computer chooses a number between 1 - 100, asks the player to choose a number in the same range and type it in, and finally the computer will check if they match.

The second batch of lines are for the scenario of the player guessing the number correctly, the game will tell them they are correct, and ask if they wnat to play again, if the player says no, the game ends, if they say yes then the whole process starts again.

The last batch are for when the player guesses wrong, and depending if the number the player chose is higher or lower than the computers', the player will be informed to guess lower or higher and the player would then have to type their number again.
