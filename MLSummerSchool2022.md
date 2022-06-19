<div align="center">

<a href="https://www.amazon.com">
<img src="https://upload.wikimedia.org/wikipedia/commons/a/a9/Amazon_logo.svg" width="300" alt="Amazon Logo">
</a>

# Amazon ML Summer School 2022
## Edition 2 • Programming Questions

Documentation and analysis for the programming questions asked during **Amazon ML Summer School 2022 (Edition 2)**.

<br>

<img src="https://ziadoua.github.io/m3-Markdown-Badges/badges/AWS/aws1.svg">
<img src="https://ziadoua.github.io/m3-Markdown-Badges/badges/C++/c++2.svg">
<img src="https://ziadoua.github.io/m3-Markdown-Badges/badges/LeetCode/leetcode2.svg">
<img src="https://m3-markdown-badges.vercel.app/stars/3/3/cu-sanjay/Amazon-ML-Summer-School-2026">

<br><br>

<img src="https://img.shields.io/badge/Edition-2022-ff7f50?style=for-the-badge&logo=readme&logoColor=white&labelColor=2c3e50">
<img src="https://img.shields.io/badge/DSA%20Questions-2-6a5acd?style=for-the-badge&logo=codeforces&logoColor=white&labelColor=2c3e50">
<img src="https://img.shields.io/badge/Language-Java%20%7C%20Python%20%7C%20C++-00bfff?style=for-the-badge&logo=python&logoColor=white&labelColor=2c3e50">

</div>

> [!IMPORTANT]
>
> These are the programming questions from **Amazon ML Summer School 2022 – Edition 2**. [⭐ Star the repository](https://github.com/cu-sanjay/Amazon-ML-Summer-School-2026) and jump into some practice questions on LeetCode.

## Navigation

- [Overview](#overview)
- [Programming Questions](#programming-questions)
  - [Question 1 • Three Robots](#question-1--three-robots)
  - [Question 2 • Mean-Median-and-Mode](#question-2--mean-median-and-mode)
- [LeetCode Practice](#leetcode-practice)

## Overview

Amazon ML Summer School assessments emphasize:

- Problem solving
- Greedy algorithms
- Data structures
- Mathematical reasoning
- Time and space complexity analysis

This repository serves as concise documentation for the questions from **Edition 2**.

## Programming Questions

| No. | Question | Primary Topic |
| :-- | :------- | :------------ |
| **1** | Three Robots | Greedy, Stack, Lexicographical Ordering |
| **2** | Mean, Median and Mode | Arrays, Sorting, Frequency Counting |

# Question 1 • Three Robots

> [!NOTE]
>
> **Primary Topics**
>
> - Greedy Algorithm
> - Stack
> - Lexicographical Ordering
> - String Processing

## Problem Statement

There are three robots named **Ray**, **Ben**, and **Kevin**.

Initially:

- Ray contains a string **S** of length **N**.
- Ben contains an empty string.
- Kevin contains an empty string.

Two operations are allowed.

### Move 1

Remove the **first character** from Ray and append it to the end of Ben.

### Move 2

Remove the **last character** from Ben and append it to the end of Kevin.

The operations continue until both Ray and Ben become empty.

The objective is to obtain the **lexicographically smallest possible string** in Kevin.

### Illustration

```text
Initially

Ray    : abcxyz
Ben    :
Kevin  :

Move 1

Ray    : bcxyz
Ben    : a
Kevin  :

Move 2

Ray    : bcxyz
Ben    :
Kevin  : a
```

The order of operations determines the final string, making the problem an optimization task rather than a simple simulation.

<details>

<summary><strong>Key Observation</strong></summary>

Ben behaves exactly like a **stack**.

- Characters are inserted only at the end.
- Characters are removed only from the end.

At every step, the decision is whether to:

- Continue pushing characters into the stack, or
- Pop characters immediately into Kevin.

The optimal decision depends on whether a smaller character still exists later in Ray.

Therefore, keeping track of the **minimum remaining character** in every suffix allows optimal greedy decisions.

</details>

<details>

<summary><strong>Approach</strong></summary>

The solution combines two ideas.

### Greedy Strategy

Always output the smallest possible character as early as possible.

### Stack Simulation

Ben naturally behaves like a stack.

### Suffix Minimum Array

Before processing the string, compute the minimum character available from every suffix.

This allows each decision to be made in constant time.

The overall algorithm performs only one traversal while maintaining optimal lexicographical ordering.

</details>

<details>

<summary><strong>Algorithm</strong></summary>

1. Compute the smallest character for every suffix of the string.
2. Traverse the string from left to right.
3. Push every incoming character onto Ben.
4. Compare the top of Ben with the smallest remaining character in Ray.
5. Pop whenever doing so cannot make the answer larger.
6. Continue until Ray becomes empty.
7. Finally, pop all remaining characters from Ben.

</details>

## Complexity

| Metric | Complexity |
| :----- | :--------- |
| Time Complexity | **O(N)** |
| Space Complexity | **O(N)** |

> [!TIP]
>
> Although the problem involves three different strings, the effective data structure is simply a **stack**, making the solution linear in both time and space.

## Related LeetCode Problem

**Using a Robot to Print the Lexicographically Smallest String**

https://leetcode.com/problems/using-a-robot-to-print-the-lexicographically-smallest-string/

> [!NOTE]
>
> This LeetCode problem follows the same underlying greedy and stack-based concept and is excellent practice for understanding the optimization strategy used in this Amazon question.

# Question 2 • Mean, Median and Mode

> [!NOTE]
>
> **Primary Topics**
>
> - Arrays
> - Sorting
> - Mathematical Computation
> - Frequency Counting

## Problem Statement

Given an integer `input1` representing the number of elements and an integer array `input2`, compute the following statistical values:

- Mean
- Median
- Mode

The returned values for **mean** and **median** must be accurate up to **six decimal places**.

If multiple numbers share the highest frequency, the **smallest value** must be selected as the mode.

### Definitions

<details>
<summary><strong>Mean</strong></summary>

The **mean** represents the arithmetic average of all elements.

```text
Mean = (Sum of all elements) / Number of elements
```

Example

```text
Input

1 2 3

Mean

(1 + 2 + 3) / 3 = 2
```

</details>

<details>
<summary><strong>Median</strong></summary>

The **median** represents the middle value after sorting the array.

If the number of elements is odd,

```text
Median = Middle Element
```

If the number of elements is even,

```text
Median = Average of the two middle elements
```

Example

```text
Input

9 3 5 1 7

Sorted

1 3 5 7 9

Median

5
```

</details>

<details>
<summary><strong>Mode</strong></summary>

The **mode** is the value that appears most frequently.

When multiple values have the same maximum frequency, choose the **smallest value**.

Example

```text
Input

5 4 5 3 3

Frequency

3 → 2
5 → 2
4 → 1

Mode

3
```

</details>

<details>
<summary><strong>Approach</strong></summary>

The solution is divided into three independent computations.

### Mean

- Traverse the array once.
- Compute the total sum.
- Divide the sum by the number of elements.

### Median

- Sort the array.
- Return the middle element for odd-sized arrays.
- Return the average of the two middle elements for even-sized arrays.

### Mode

- Count the frequency of every element.
- Identify the highest frequency.
- If multiple elements have the same frequency, return the smallest one.

</details>

<details>
<summary><strong>Algorithm</strong></summary>

1. Read the array.
2. Compute the sum of all values.
3. Calculate the mean.
4. Sort the array.
5. Calculate the median.
6. Count the frequency of every element.
7. Select the smallest element having the highest frequency.
8. Return the three computed values.

</details>

## Complexity

| Metric | Complexity |
| :------ | :--------- |
| Mean | **O(N)** |
| Median | **O(N log N)** |
| Mode | **O(N)** |
| Overall | **O(N log N)** |

> [!TIP]
>
> The sorting step dominates the overall complexity, making the complete solution **O(N log N)**.

## Sample Examples

<details open>

<summary><strong>Example 1</strong></summary>

### Input

```text
N = 3

Array = {1, 2, 3}
```

### Output

```text
Mean   = 2.000000

Median = 2.000000

Mode   = 1
```

</details>

<details>

<summary><strong>Example 2</strong></summary>

### Input

```text
N = 5

Array = {41, 18467, 6334, 26500, 19169}
```

### Output

```text
Mean   = 14102.200000

Median = 18467.000000

Mode   = 41
```

</details>

# LeetCode Practice

> [!IMPORTANT]
>
> Amazon did not publish official editorials for these questions. The following LeetCode problems cover the same concepts and are recommended for additional practice.

<!-- Question 1 -->
<h2>Question 1 • Three Robots</h2>
<table style="border-collapse: collapse; border-radius: 8px; overflow: hidden; width: 100%; text-align: left; font-family: Arial, sans-serif;">
  <thead style="background: #2c3e50; color: #fff;">
    <tr>
      <th style="padding: 10px;">Problem</th>
      <th style="padding: 10px;">Difficulty</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #ecf0f1;">
      <td style="padding: 10px;">
        <a href="https://leetcode.com/problems/using-a-robot-to-print-the-lexicographically-smallest-string/" target="_blank" style="color: #2980b9; text-decoration: none; font-weight: bold;">
          Using a Robot to Print the Lexicographically Smallest String
        </a>
      </td>
      <td style="padding: 10px; color: #e74c3c; font-weight: bold;">Hard</td>
    </tr>
  </tbody>
</table>

<!-- Question 2 -->
<h2>Question 2 • Mean, Median and Mode</h2>
<table style="border-collapse: collapse; border-radius: 8px; overflow: hidden; width: 100%; text-align: left; font-family: Arial, sans-serif;">
  <thead style="background: #2c3e50; color: #fff;">
    <tr>
      <th style="padding: 10px;">Topic</th>
      <th style="padding: 10px;">Practice</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #ecf0f1;">
      <td style="padding: 10px;">Sorting</td>
      <td style="padding: 10px;">
        <a href="https://leetcode.com/problems/sort-an-array/" target="_blank" style="color: #27ae60; font-weight: bold;">Sort an Array</a>
      </td>
    </tr>
    <tr style="background: #f9f9f9;">
      <td style="padding: 10px;">Frequency Counting</td>
      <td style="padding: 10px;">
        <a href="https://leetcode.com/problems/top-k-frequent-elements/" target="_blank" style="color: #27ae60; font-weight: bold;">Top K Frequent Elements</a>
      </td>
    </tr>
    <tr style="background: #ecf0f1;">
      <td style="padding: 10px;">Arrays</td>
      <td style="padding: 10px;">
        <a href="https://leetcode.com/problems/majority-element/" target="_blank" style="color: #27ae60; font-weight: bold;">Majority Element</a>
      </td>
    </tr>
    <tr style="background: #f9f9f9;">
      <td style="padding: 10px;">Mathematical Operations</td>
      <td style="padding: 10px;">
        <a href="https://leetcode.com/problems/find-the-pivot-integer/" target="_blank" style="color: #27ae60; font-weight: bold;">Find the Pivot Integer</a>
      </td>
    </tr>
  </tbody>
</table>

> This repository is intended for educational purposes only.

<div align="center">

### Amazon ML Summer School 2022 • Edition 2

Documentation • Algorithms • Complexity Analysis • Practice Resources

</div>