# EGchallenge

Make a Word

In this challenge, you'll build a word-guessing game like Scrabble or Boggle.

The idea for this game is simple: players have to make words out of a set of letters shown on the screen.

There is only one rule: words must use only the letters shown in the set.

For example, if the letters shown are N A I P L R A, then the following words are correct: PLAN, AIR, RAIN.

The following words are incorrect: APE (E is not one of the provided letters) and NARWHAL (no W or H).

Your task is to build a working version of this game with HTML, CSS, and JavaScript.

Here's an example of what the basic version could look like:

example game gif

Getting Started

Sign up for a free CodePen account.
Open the starter code for the challenge.
Click the Fork button at the top. Now your edits and progress can be saved to your own CodePen account.
Note: to avoid losing your work, you will want to save frequently.

Running Tests

This challenge comes with its own suite of tests, which means that you can see which objectives you've completed by running the tests.

To run your tests, open the "Console" with the button at the bottom, and execute the function runTests().

Of course, at the start most of these tests will be failing, because you haven't written code to make them pass. As you complete the objectives, however, you should see more and more green (green = passing).

Run your tests frequently! They're a great way to tell if you're on-track.

Note: these tests only test your JavaScript code, not your HTML + CSS. If the objective includes HTML + CSS components, you can't rely on the tests to tell you if you've completed the objective or not. For that, you'll have to read the objective itself.

Challenge Objectives

Complete each of the challenge objectives in order.

1: Complete the Logic in checkGuess()

STOP! This step has already been completed for you. The developer who solved it even recorded this video for you to watch so you can get up-to-speed.

As you watch the video, note things like:

Which steps they go through to solve the problem
How they use pseudocode to guide their development process
How they use the console and the tests to verify their code
Any additional work they do beyond the tests
Objective 1, which has been completed for you is defined below:

The incomplete logic in the checkGuess() function needs to be finished in order for the basic version of this game to work.

Tasks:

 Write the body code of the checkGuess() function so that it satisfies its description (provided in a comment just above the function declaration).
 Make sure that checkGuess() notifies the user of correct and incorrect guesses.
2: Change the Letters from JavaScript

Having a single, static set of letters is not that interesting. Eventually, we'll need to change the letter set so that players can make different words.

The first step is to create a function in JavaScript that can change the letters displayed in HTML.

Tasks:

 Create a new function in your JavaScript file called updateLetters().
 Inside this function, define a variable newLetters and set it to the string "ABCD".
 This function should update the contents of the <div> with id letters with the string in newLetters.
For example, running updateLetters() should change the content of the letters <div> tag to ABCD.

Once you write your function, test it out in the Console. Run the tests to see if you successfully implemented this function.

3: Make a "Random Generate" Feature

To make the game more interesting, a player should be able to generate a new random set of letters.

Tasks:

 Create a new function called randomLetters() that returns a string of 7 random letters from A to Z.
 Make sure that randomLetters() always returns a string with at least 2 vowels (otherwise it will be hard to make any words).
 Change the updateLetters() function from the last objective so that it generates a new set of random letters and updates the HTML to display them.
 Make a <button> that, when clicked, runs the function updateLetters().
If you're not sure how to generate random letters from JavaScript, the internet has many answers! Use your Google skills to find examples, but be sure to read and test them before pasting them into your code. Run the tests to check on your progress.

4: Improve the User Interface

The current user interface (or UI, for short) is not very pretty. There is very little styling added to make it look better than the default.

Tasks:

 Write CSS (and HTML, if necessary) to make your page look nicer.
If you want inspiration, you can start by trying to re-create this style:

example improved ui

5: Make a "Shuffle" Feature

Another common feature of word games is the "shuffle" button, which shuffles the order of the letters to make it easier to spot words that may be hidden within.

Tasks:

 Implement a "shuffle" feature for your game.
 Write a JavaScript function called shuffle() that takes a string and returns a new string with the characters shuffled.
 Add a user interface element to let players shuffle the letters by clicking a button.
For example, the shuffle() function should work like this:

shuffle("abcd"); // => "cbad"

// so you could assign the return value of this function like this:

var originalString = "original";
var shuffledString = shuffle(originalString);
console.log(shuffledString); // prints "larinigo"
This objective is a bit harder. You'll have to figure out what it means to "shuffle" a set of characters in a string.

Make sure to work out the logic for your procedure before coding it, and test your code as you go along. Run the tests to check your progress.

6: Get Creative

What else can you do to improve the game? What other features would you like to build?

Some ideas:

Make a scorecard that tracks correct and incorrect guesses.
Make the number of letters adjustable (i.e. can choose from more or fewer than 7 letters).
Improve the "randomness" of your randomLetters() function. A good word puzzle game will give you X's and Z's less often than D's and P's. Assign different probabilities for the letters of the alphabet.
Assign number values to letters (like in Scrabble) and calculate a player's score using them.
Improve the checkGuess() function to check if the word entered is actually a real English word. You might need to use a library or an API to accomplish this.
This objective is intentionally open-ended. There are no tests (unless you want to write some of your own ;). Have fun with it!

Saving your Code

Once you are finished, you will probably want to save your code for your own keeping.

While you can save your code wherever you like, we recommend using GitHub Gist (you'll need a GitHub account). You can copy and paste your HTML, CSS, and JavaScript into their own files in a gist.
