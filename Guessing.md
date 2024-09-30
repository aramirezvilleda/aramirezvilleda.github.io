***mermaid

flowchart TD
	A([Start])-->B[(Computer Chooses Number Between 1-100])
	B --> C([Ask Player to Guess a Number Between 1 - 100])
	C --> D([Player Inserts Number])
	D --Computer Compares Numbers--> E([Do They Match?])
	E --Yes--> F([Display: YOU WIN!])
	F --> G([End])
	H --No-->I(Is the Players Number Higher than the Computer's?])
	I --No--> J([Display: Guess Higher!])
	J --> B
	I --Yes--> K([Guess Lower!])
	K --> B
***


