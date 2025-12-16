
# Hello, World Program (Python)

## Lab Overview

Welcome to **Introduction to Programming**. In this lab, you will use the **Python programming language** to write and run your first program using the **AWS Cloud9 IDE**.

The purpose of this lab is to confirm that the Python development environment is set up correctly.

**Estimated completion time:** 45 minutes

---

## Accessing the AWS Cloud9 IDE

1. Choose **Start Lab** at the top of the lab instructions.
2. Wait until the message **Lab status: ready** appears, then close the panel.
3. Choose **AWS** to open the AWS Management Console.
4. Navigate to **Services > Cloud9**.
5. Locate **reStart-python-cloud9** under *Your environments*.
6. Choose **Open IDE**.

**Notes:**

* Allow pop-ups if prompted by your browser.
* If you see prompts about project settings or third‑party content, choose **Discard** or **No**.

---

## Creating the Python Exercise File

1. In the Cloud9 menu, choose **File > New From Template > Python File**.
2. Delete the sample code in the new file.
3. Choose **File > Save As...**
4. Name the file `hello-world.py`.
5. Save it in:

   ```
   /home/ec2-user/environment
   ```

---

## Accessing the Terminal Session

1. Choose the **+** icon in the IDE.
2. Select **New Terminal**.
3. Verify your working directory:

   ```bash
   pwd
   ```

   Expected output:

   ```
   /home/ec2-user/environment
   ```

---

## Exercise 1: Introducing Python

Python is a **high-level, general-purpose programming language** used for applications such as websites, automation, and desktop software.

This lab uses **Python 3.6.x**.

### Checking Python Versions

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
4. Choose the **Run (▶)** button.
5. Confirm the output displays:

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

* Accessed AWS Cloud9
* Verified Python installation
* Written and executed your first Python program

🎉 **Congratulations on completing your first Python lab!** 🎉

---

## Program

AWS re/Start – Introduction to Programming
