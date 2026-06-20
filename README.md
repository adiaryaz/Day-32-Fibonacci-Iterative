# Day-32-Fibonacci-Iterative
Day 32/100 - Python Program to Find the Fibonacci Series Without using Recursion

# Find Fibonacci Series (Iterative)
A program to generate and display the Fibonacci series up to a specified number of terms utilizing a highly efficient iterative approach.

## 📝 Description

This program calculates the **Fibonacci series**, a sequence where each number is the sum of the two preceding ones, starting with 0 and 1.

Unlike the recursive approach (which can be slow and memory-intensive for large numbers), this script uses an **iterative** method. It utilizes a `for` loop and Python's simultaneous variable assignment (`a, b = b, a + b`) to efficiently update the terms in a single step without needing temporary variables. Instead of printing the numbers one by one, it collects them into a Python `list` and returns the complete array at the end of the calculation.

---

## 🎯 Problem Statement

### Input:

* **Input 1:** A single integer representing the total number of terms (`num_terms`) to generate in the sequence.

### Output:

* If the input is valid, a prefix text: "Fibonacci series:" followed by a Python list containing the generated sequence on the next line.
* If the input is zero or negative, an error message: "Please enter a positive integer."

### Rules:

1. The program must accept an integer input from the user representing the number of terms.
2. The program must evaluate if the input is valid (`num_terms > 0`). If not, handle the error gracefully.
3. The program must utilize an iterative function (`fibonacci_series`) with a `for` loop to calculate the sequence.
4. Initialize two variables `a` and `b` to `0` and `1`, respectively.
5. In each iteration, append `a` to a result list, then update `a` to the current value of `b`, and `b` to the sum of the old `a` and `b`.
6. Return the finalized list and print it.

---

## 💡 Examples

### Example 1 (Standard Sequence)

**Input:**

```
5


```

**Output:**

```
Fibonacci series:
[0, 1, 1, 2, 3]


```

**Explanation:** The loop iterates 5 times. It collects the values of `a` successively: 0, 1, 1, 2, and 3, storing them safely in a list before printing.

### Example 2 (Extended Sequence)

**Input:**

```
8


```

**Output:**

```
Fibonacci series:
[0, 1, 1, 2, 3, 5, 8, 13]


```

**Explanation:** The loop continues efficiently up to 8 terms, placing the sequence natively into a list structure.

### Example 3 (Single Term)

**Input:**

```
1


```

**Output:**

```
Fibonacci series:
[0]


```

**Explanation:** The user asks for exactly 1 term. The loop runs exactly once, appending `0` to the list and updating `a` and `b`, but terminates before the next append.

### Example 4 (Invalid Input)

**Input:**

```
0


```

**Output:**

```
Please enter a positive integer.


```

**Explanation:** The initial check `if num_terms <= 0:` intercepts the invalid input (0 or negative numbers) and prints the warning prompt without executing the loop.

---

## 🚀 How to Use

1. **Clone this repository** (or save the script)

```bash
git clone https://github.com/adiaryaz/Day-32-Fibonacci-Iterative.git
cd fibonacci-iterative


```

2. **Run the program**:

```bash
python main.py


```

Enter the number of terms when prompted to see the Fibonacci series generated efficiently as a list.
