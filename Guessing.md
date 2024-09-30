```mermaid

graph TD;
	A([Start])  ----> B([Computer chooses number between 1-100]);
    B ----> C([Game instructs: **_Choose a number between 1-100_**]);
    C -- The player inserts their number --> D([Computer compares the numbers]);
    D ----> E([Do they match?]);

    E -- Yes --> F([Game Displays: **_CORRECT_**!]);
    F ----> G([Game asks: **_TRY AGAIN?_**]);
    G -- Yes --> B;
    G -- No --> H([End]);

    E -- No --> I([Is the player's number higher than the computers'?]);
    I -- Yes --> J([Game instructs: **_GUESS LOWER!_**]);
    J ----> C;
    I -- No --> K([Game instructs: **_GUESS HIGHER!_**]);
    K ----> C;

```

When the game starts, the computer will choose a random number between 1 and 100.

Then the game will tell the player to choose a number in the same range.

Once the players inserts their number, the computer will compare both numbers to see if they match.

* If they do, the game will tell the player they are correct and ask if they want to play again. If they don't want to, the game ends. If they do, they are the whole process starts over.

* If the numbers don't match, the computer will see if the player's num,ber is higher or lower that the computer's.
	* If it's higher, the game will tell the player to guess a number lower than the one before and are asked to type it in again.
	* If it's lower, than the payer is told to choose a number higher than the before, and are asked to type in their number again.
