<div align="center">

# Amazon ML Summer School 2024  
## Hands-On Programming Questions (Slot 4)

</div>

<div>
  <img
    src="https://github.com/user-attachments/assets/2cba809d-fe9c-4d57-8b46-c741cae01df3"
    alt="Amazon ML Summer School"
    width="120"
    align="left"
  />

  <p align="right" style="margin-top:30px;">
    <strong>Date:</strong> June 23, 2024
  </p>
</div>

<br clear="all">

## Question 1: Nearest Friend's House

<details>
<summary><strong>View Question</strong></summary>

<p align="center">

![](https://github.com/user-attachments/assets/ea747fc8-ef91-4b4f-ac92-bb9cb294fed7)

</p>

</details>

You are given an integer array **A** of size **N**, where every element is **distinct** and represents the x-coordinate of a friend's house.

For example:

```text
A = [1, 3, 8]
```

means there are friends living at:

- x = 1
- x = 3
- x = 8

The array is guaranteed to be sorted in ascending order.

### Problem Statement

Each friend's house has a maximum capacity of **N - 1** people.

Every friend wants to host a gathering and invite exactly **N - 2** friends.

To minimize overall travel, the host always invites the **N - 2 closest friends**, so that the **total distance traveled** by all invited friends is as small as possible.

For every friend, return the minimum total distance traveled by the invited guests.

### Input

- `input1`: Integer `N`
- `input2`: Integer array `A`

### Output

Return an integer array where the `i-th` value represents the minimum total distance traveled when the `i-th` friend is the host.

### Example

#### Input

```text
N = 5
A = [1, 2, 3, 4, 5]
```

#### Output

```text
[6, 4, 4, 4, 6]
```

### Explanation

**Host = 1**

Invites:

- 2
- 3
- 4

Distance:

```text
(2-1) + (3-1) + (4-1) = 6
```

**Host = 2**

Invites:

- 1
- 3
- 4

Distance:

```text
(2-1) + (3-2) + (4-2) = 4
```

**Host = 3**

Invites:

- 1
- 2
- 4

Distance:

```text
(3-1) + (3-2) + (4-3) = 4
```

**Host = 4**

Invites:

- 2
- 3
- 5

Distance:

```text
(4-2) + (4-3) + (5-4) = 4
```

**Host = 5**

Invites:

- 2
- 3
- 4

Distance:

```text
(5-2) + (5-3) + (5-4) = 6
```

>[!TIP]
> To better understand how the algorithm chooses the closest **N-2** friends and computes the minimum total distance, **try the interactive visualization below.**

![Nearest Friend’s House Visualization](https://raw.githubusercontent.com/cu-sanjay/HostSVG/refs/heads/main/Nearest_Friends.svg)

## Similar Practice Problems

| Platform   | Problem                                                                 | Why it is Similar                                |
|------------|-------------------------------------------------------------------------|--------------------------------------------------|
| LeetCode   | [658. Find K Closest Elements](https://leetcode.com/problems/find-k-closest-elements/) | Closest element selection around a target        |
| LeetCode   | [2602. Minimum Operations to Make All Array Elements Equal](https://leetcode.com/problems/minimum-operations-to-make-all-array-elements-equal/) | Prefix sums and distance calculations            |
| LeetCode   | [296. Best Meeting Point](https://leetcode.com/problems/best-meeting-point/) | Distance minimization                            |
| LeetCode   | [849. Maximize Distance to Closest Person](https://leetcode.com/problems/maximize-distance-to-closest-person/) | Distance-based reasoning                         |
| HackerRank | [Closest Numbers](https://www.hackerrank.com/challenges/closest-numbers/problem) | Adjacent distance computation                    |
| HackerRank | [Sherlock and MiniMax](https://www.hackerrank.com/challenges/sherlock-and-minimax/problem) | Distance optimization on a number line           |


# Question 2: Pair Problem

<details>
<summary><strong>View Question</strong></summary>

<p align="center">

![](https://github.com/user-attachments/assets/bff593bc-0935-40a2-9e84-ad43b4db3ae5)

</p>

</details>

Lucy has an integer array **A** of size **N**.

All elements are **distinct**.

She may perform the following operation any number of times:

Choose two elements **x** and **y** such that

```text
LCM(x, y) × HCF(x, y)
```

is also present in the array.

Return the **maximum number of valid ordered pairs (x, y)**.

>[!NOTE]
>
> Using the identity:
>
> ```text
> LCM(x, y) × HCF(x, y) = x × y
> ```
>
> the problem simplifies to:
>
> Find all ordered pairs `(x, y)` such that
>
> ```text
> x × y
> ```
>
> exists in the array.

Also note:

```text
(x, y) ≠ (y, x)
```

Both are counted separately.

### Input

- `input1`: Integer `N`
- `input2`: Integer array `A`

### Output

Return the maximum number of valid ordered pairs.

### Example

#### Input

```text
N = 5
A = [1, 2, 3, 4, 5]
```

#### Output

```text
10
```

### Explanation

Valid ordered pairs are:

```text
(1,1)
(1,2)
(2,1)
(1,3)
(3,1)
(1,4)
(4,1)
(1,5)
(5,1)
(2,2)
```

Hence,

```text
Answer = 10
```

## Similar Practice Problems

| Platform   | Problem                                                                 | Why it is Similar                                |
|------------|-------------------------------------------------------------------------|--------------------------------------------------|
| LeetCode   | [1726. Tuple with Same Product](https://leetcode.com/problems/tuple-with-same-product/) | Product hashing (closest match)                  |
| LeetCode   | [2183. Count Array Pairs Divisible by K](https://leetcode.com/problems/count-array-pairs-divisible-by-k/) | Pair counting using number theory                |
| LeetCode   | [2001. Number of Pairs of Interchangeable Rectangles](https://leetcode.com/problems/number-of-pairs-of-interchangeable-rectangles/) | Hash map based pair counting                     |
| LeetCode   | [1497. Check If Array Pairs Are Divisible by k](https://leetcode.com/problems/check-if-array-pairs-are-divisible-by-k/) | Pair formation using mathematical properties     |
| HackerRank | [Pairs](https://www.hackerrank.com/challenges/pairs/problem)            | Efficient pair counting                          |
| HackerRank | [Count Triplets](https://www.hackerrank.com/challenges/count-triplets/problem) | Hashing and frequency optimization               |

> [!IMPORTANT]
> For the complete **2024 Machine Learning Questions** and **additional 2024 Hands-On Programming Questions**, refer to:
>
> **Amazon ML Summer School 2024 ML Assessment PDF**
>
> [ML Summer School 2024](https://github.com/cu-sanjay/Amazon-ML-Summer-School-2026/blob/main/MLSummerSchool2024.pdf)