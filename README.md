# Problem Set 8

### Due Tuesday, April 6, 2021, at 11:59pm EST

For this problem set, you will submit to Canvas **a single .zip file**. Detailed instructions for what the .zip file should contain are at the end of this problem set. Note that if you do not submit the files as specified here, there will be a major deduction in your grade for this assignment. Following directions to the letter is a crucial skill for computer programming.

**Structure:** Your programs should all have the following format: import statements (if necessary); the global variables (if there are any); then function definitions (if there are any); then a `main()` function that gets the ball rolling and calls the functions you defined (if any); and finally outide all other functions, the call to `main()`.

**Comments:** I now expect you to write comments in your code! Two points will be deducted if you provide no or minimal comments, and 1 point will be deducted if you have sufficient comments but they do not conform to the requirements outlined in PS4.

**Folders:** Make sure your programs and your files are all in the same folder. Download this whole directory to your desktop, unzip it, and write all of yoru programs in that folder.

**Honor pledge**: And, as always, in every program, the first four lines (comments) should be your honor pledge.

## Part 1: Cereal data
read in data using csv and save all of the numeric values into a numpy array
use numpy to find cereals whose protein content > something
convert to percentages and find top 5 most sugary
print out a histogram of calories


## Part 2: Number guessing
In `part2.py`, I have provided the code for guessing a number between 1 and 100 using the three techniques we have discussed and coded up ourselves, with one function for each of the three techniques. Eacn function takes the number to be guessed as an argument and then returns the number of guesses required to guess that number correctly using of the three techniques:

* start guessing at 1 and go up to 100 until you guess the right number
* guess random numbers, never guessing the same number twice, until you guess the right number
* binary search

You will write a function, `simulateguessing(technique)` whose argumment, `technique` is a string that is either "ordered", "random", or "binarysearch". This function will have a loop that generates a randon number between 1 and 100 and then calls the guessing function corresponding to the technique specified by the argument 1000 times. It will save each number it gets back from the guessing function into a list, so that at the end of the loop, it will have a list 1000 elements long containing the number of guesses required for each random number it generated. It will return that list.

Finally in your `main()` function, you will do the following:

* Call `simulateguessing()` with each of the three possible values ("ordered", "random", or "binarysearch"), saving the results out to three separate lists. 
* Using `numpy`, calculate the mean, min, max, and standard deviation for each list, and print it out.
* Using `matplotlib`, create a plot with three subplots, where each subplot contains a histogram for one of the three lists you got back from `simluateguessing()`. 

Here is some sample output, and the subplots that I got.

plot the number of guesses it takes for each of the three guessing techniques, draw a line at the average

