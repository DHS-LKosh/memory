# Memory Game Assignment

## Overview
**Concentration**, also known as Matching Pairs, Match Match, Match Up, Memory, Pleonasm, Shank, Pexeso or simply Pairs, is a card game in which all of the cards are laid face down on a surface and two cards are flipped face up over each turn. The object of the game is to turn over pairs of matching cards.

You can play an example of a memory game here: https://www.helpfulgames.com/subjects/brain-training/memory.html

## Requirements
* Use a **2D Array** called **cards** for storing the values of the cards (emojis). Each card will contain a String with an emoji. Remember you need two copies of each emoji for the game to work.
* You need to have at least 5x6 elements.
* Use a **2D Array** of booleans called **isShown** to store whether each card is revealed. This should be a parallel array to cards.
* A **void method** called **shuffleArray()** which will randomly exchange elements until you are satisfied with the shuffling.You may also want to reset isShown in this method.
  * To shuffle the array, generate two sets of row and column numbers, and exchange the elements. Loop to repeat until you are happy with the shuffle. You may NOT use any built-in shuffling methods. This must be done manually.
* A **void method** called **isDone()** which returns a boolean indicating whether the game is over or not.	
* A **void method** called **displayBoard()** which will display the cards similar to the layout shown on the below.
  * Use the **overloaded method** to accept two additional integer parameters - one row, column, to use to display the user’s chosen cell without changing the value of the isShown() value for the cell. I overloaded this method twice, so I could handle the two user choices.
* A **boolean method** called **isValid()** which will return true or false depending on whehter the cell choosen by the user has not already been choosen (isValid()=true)
* In your **psvm**, Write a game loop that will:  
  * Show the board
  * Accept user input in the form of a row & column number.  **ERROR TRAP** user input.
  * Show the first card chosen
  * Accept user input in the form of a row & column number.  **ERROR TRAP** user input.
  * Show the second card chosen
  * Check whether the two cards are a match. 
  * If the cards match, set the corresponding isShown elements to true.  If they do not match, flip the cards back over so the contents are not visible.
  * Check if the game is won
  * If the game is over, see if the user wants to play again and reset the game

