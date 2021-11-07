# Hangman-game

### What is Hangman about?
Refer to this wikipedia [link](https://en.wikipedia.org/wiki/Hangman_(game)). One player (computerized) thinks of a word and the other player will have to try and guess it. The word to be guessed will be shown as a row of underscores/dashes.

<img src="https://upload.wikimedia.org/wikipedia/commons/d/d6/Hangman-6.png"/>

eg. If the word to be guessed has 4 letters, it will be shown as such _ _ _ _

---

### Rules of Hangman

Player can either input a letter or a word.

- If player inputs a letter:  
  - Input only valid if it is a letter from A-Z
  - Loses a life if letter is incorrect

- If player inputs a word: 
  - Input is only valid if it has same number of letters as the word
  - Loses a life if word is incorrect

---

### Task 1

Create a function to select a random word.

- Create a list `words` to store words from A-Z.   
https://www.randomlists.com/data/words.json


- Create function `select_a_word()` to select a random word 
from the list.<br /> 
Hint: `random.choice()` is a built-in python function which returns a randomly selected word from the list

---

### Task 2

Create a function `hangman()` whereby users can play the game. <br /> 
Hint: A while loop is required

Do take into consideration the different cases:
- When player gives an input<br /> 
- Keeping track of the game progress


**1. When player gives an input**
- Scenario 1 - Player inputs a letter 
  - If `guessed letter` is not a valid letter
  - If `guessed letter` was guessed previously
  - If `guessed letter` is in `word`
  - If `guessed letter` not in `word`

- Scenario 2 - Player inputs the full word 
  - If the `guessed word` is the same as `word`

- Scenario 3 - Player either inputs more or fewer letters than the number of letters in the word

**2. Keeping track of game progress**
- Scenario 1 - When `word` is still being guessed
- Scenario 2 - When `word` has been guessed
- Scenario 3 - When player is out of `lives`

--- 

### Task 3 

Additional Challenge: Create a function `play_again()` to give users the option to replay the game.

--- 

### Game Snippets
- Word is guessed <br />

![hangman2](https://user-images.githubusercontent.com/92679068/140646221-65789fd9-a305-449e-b323-6915167a784b.JPG)

---

- Letter was previously guessed <br />

![hangman3](https://user-images.githubusercontent.com/92679068/140646228-c5e9eb2f-11fc-4abf-8020-d12decd56800.JPG)

---

- Player out of guesses <br />

![hangman4](https://user-images.githubusercontent.com/92679068/140646229-536b0f6d-184c-4314-b315-93e1b0e5d6c1.JPG)

---

- invalid input <br />

![hangman6](https://user-images.githubusercontent.com/92679068/140646232-1dbbb4b2-05ea-4af5-ab65-226e5ed0bb14.JPG)

---

- length of guess is incorrect <br />

![hangman7](https://user-images.githubusercontent.com/92679068/140646235-bd8cc0ac-efe3-49a2-a817-13de68803513.JPG)

---
