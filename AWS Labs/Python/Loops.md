

---

# Working with Loops – Python Lab

## Lab Overview

This lab introduces **loops in Python**, which are used to repeat a block of code. Two types of loops were covered:

* **while loop**
* **for loop**

The lab was completed using the **AWS Cloud9 IDE** as part of the AWS re/Start program.



---

## Objectives

By completing this lab, I learned how to:

* Use a **while loop** to repeat code until a condition is met
* Use a **for loop** to iterate through a sequence of numbers
* Generate random numbers using the `random` module
* Accept and process user input
* Write basic pseudocode
* Add comments to Python code for readability

---

## Environment Used

* **Platform:** AWS Cloud9
* **Language:** Python 3
* **Directory:** `/home/ec2-user/environment`

---

## Exercise 1: While Loop – Guess the Number Game

### Description

This script creates a simple game where the computer randomly selects a number between 1 and 10, and the user keeps guessing until the correct number is entered.


### File

* `while-loop.py`

### Program Logic (Pseudocode)

1. Generate a random number between 1 and 10
2. Set a variable to track if the guess is correct
3. While the guess is not correct:

   * Ask the user for a guess
   * Compare the guess to the random number
   * If correct, display a success message and stop the loop
   * If incorrect, ask the user to try again

---

## Exercise 2: For Loop – Counting to 10

### Description

This script uses a `for` loop to count from 0 to 10 and print each number.

### Key Concepts Used

* `for` loop
* `range()` function
* Loop variables
* Indentation in Python

### File

* `for-loop.py`

### Explanation

The `range(0, 11)` function generates numbers starting from 0 up to (but not including) 11.
Each number is stored in the variable `x` and printed to the screen during each loop iteration.

---

## Sample Output

### Guess the Number Game

```
Welcome to Guess the Number!
The rules are simple. I will think of a number, and you will try to guess it.
Guess a number between 1 and 10: 5
You guessed 5. Sorry, that isn’t it. Try again.
Guess a number between 1 and 10: 7
You guessed 7. That is correct! You win!
```

### Count to 10

```
Count to 10!
0
1
2
3
4
5
6
7
8
9
10
```

---

## Conclusion

This lab helped reinforce my understanding of **looping structures in Python** and how they are used in real programs. I now understand when to use a `while` loop versus a `for` loop and how Python handles iteration and conditions.

---



