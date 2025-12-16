
# Creating a Hello, World Program (Python)

## Lab Overview

This lab introduces the basics of programming using the Python programming language. You will use the **AWS Cloud9 IDE** to create and run your first Python program.

The goal of this lab is to verify that your Python environment is set up correctly by writing and executing a simple **Hello, World** program.

**Estimated completion time:** 45 minutes

---

## Prerequisites

* An active AWS lab environment
* Access to the AWS Management Console
* Basic familiarity with using a web browser and terminal

---

## Accessing the AWS Cloud9 IDE

1. Choose **Start Lab** at the top of the lab instructions.
2. Wait until the message **Lab status: ready** appears, then close the Start Lab panel.
3. Choose **AWS** to open the AWS Management Console.
4. Navigate to **Services > Cloud9**.
5. In the **Your environments** panel, locate **reStart-python-cloud9**.
6. Choose **Open IDE**.

**Notes:**

* If prompted about pop-ups, allow them in your browser.
* If you see messages about project settings or third-party content, choose **Discard** or **No**.

---

## Creating the Python Exercise File

1. In the AWS Cloud9 IDE menu bar, choose **File > New From Template > Python File**.
2. Delete the sample code in the new file.
3. Choose **File > Save As...**
4. Name the file `hello-world.py`.
5. Save it in the directory:

   ```
   /home/ec2-user/environment
   ```

---

## Accessing the Terminal

1. In the IDE, choose the **+** icon.
2. Select **New Terminal**.
3. Confirm your working directory by running:

   ```bash
   pwd
   ```

   Expected output:

   ```
   /home/ec2-user/environment
   ```

---

## Exercise 1: Introducing Python

Python is a high-level, general-purpose programming language used for many types of applications, including web development, automation, and data analysis.

This lab uses **Python 3.6.x**.

### Checking Installed Python Versions

Run the following commands in the terminal:

```bash
python --version
python2 --version
python3 --version
```

Example output:

```text
Python 3.6.12
Python 2.7.18
Python 3.6.12
```

---

## Exercise 2: Writing Your First Python Program

1. Open the `hello-world.py` file in the IDE.
2. Enter the following code:

   ```python
   print("Hello, World")
   ```
3. Save the file (**File > Save**).
4. Choose the **Run (▶)** button near the top of the IDE.
5. Confirm the output in the bottom pane displays:

   ```text
   Hello, World
   ```

---

## Expected Output

```text
Hello, World
```

---

## Conclusion

You have successfully:

* Accessed the AWS Cloud9 IDE
* Verified the Python installation
* Created and executed your first Python program

🎉 **Congratulations on writing your first Python program!** 🎉

---

## Author

AWS re/Start – Introduction to Programming Lab
