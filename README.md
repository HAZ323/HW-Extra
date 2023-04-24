##CSE 264 – Web Systems Programming – Spring 2023
##Homework Extra Credit - Create a web version of the Simon Game
##Due May 1st @ 11:59pm. This is a firm deadline. No exceptions.

###Description
You will be implementing a web version of the game Simon, originally sold by Milton Bradley. See https://en.wikipedia.org/wiki/Simon_(game) for a description of the game.

###Architecture

This is a client only app; there is no server code. You will fill in the index.html, script.js and styles.css files.

###Instructions

1. As usual, the index.html file contains only html, the script.js file only Javascript and the styles.css file only css rules.

2. In the html file, create four squares, about an inch or so on each side, with the colors green, red, blue, yellow, arranged in a square in that order starting in the upper left corner and going clockwise. Center this square of squares on the page. Put the title "Memory Game" at the top of the page and the question "How long a sequence can you remember?" in the footer. Put a button below the four squares that says Start.

3. Write js code to do the following:

a. When the Start button is clicked, randomly select one of the four colors and play the tone associated with that color. I have provided a wav file for each color and a fifth wave file for when the player loses. At the same time that the tone is played, blank out the square for .25 seconds.

b. Wait for the the user to click the same button, and blank out the button and play the tone for the button as above. If the user clicks the wrong button, play the "lose" tone while blanking out the square and make the squares none reactive.

c. If the user clicks the correct square, then randomly pick a 2nd color and after a 2 second delay, play the tones in sequence (and hiding the corresponding squares) taking .5 seconds per color.

d. Wait for the user to click the squares in the same sequence as they were just played. Each time the user duplicates the sequence correctly, add one more color to the sequence and play them again after the 2 second delay. As above, when the user clicks a wrong square play the lose tone and make the squares non reactive.

e. Whenever the user clicks the start button, play the game over again.

4. Test until it works. How long a sequence can you remember?

5. Make sure to put in the usual comments and git add, commit, push.
