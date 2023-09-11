<div align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/a/a9/Amazon_logo.svg" alt="Amazon Logo" height="40" style="margin-right: 50px;" />
   <br>
  <img src="https://upload.wikimedia.org/wikipedia/commons/9/97/Mettl_Logo.png" alt="Mercer Mettl Logo" height="50" style="margin-left: 50px;" />
  <br><br>
  <h1>Amazon ML Summer School 2023</h1>
  <h2>Edition 3: Assessment Questions</h2>
</div>

<p align="right"><b>Date:</b> September 9, 2023</p>

<br>

## Part A: Machine Learning & Mathematics
<p><i>Basic ML concepts and Math fundamentals on topics such as Probability, Statistics, and Linear Algebra.</i></p>

<br>

**1. Probability on a Chessboard**
Two squares are chosen at random on a chessboard. What is the probability that they have a side in common?
* 8/13
* 17/18
* 5/13
* 1/18

**2. Conditional Probability**
The police plan to enforce speed limits during morning rush hour on four different routes into the city. The traps on routes A, B, C, and D are operated 40%, 30%, 20%, and 30% of the time, respectively. Biff always speeds to work, and he has a probability of 0.2, 0.1, 0.5, and 0.2 of using those routes. What is the probability that he'll get a ticket on any one morning?
* 0.27
* 0.93
* 0.73
* 0.07

**3. Variance and Correlation**
For random variables $X$ and $Y$, we have $\text{Var}(X) = 1$, $\text{Var}(Y) = 4$, and $\text{Var}(2X - 3Y) = 34$. The correlation between $X$ and $Y$ is:
* 1/2
* 1/4
* 1/3
* None of the above

**4. Bayes' Theorem**
You have two coins. One of them is fair and comes up heads with a probability of 1/2, and the other is biased and comes up heads with a probability of 3/4. You randomly pick a coin and flip it twice. You get heads both times. What is the probability that you picked the fair coin?
* 13/32
* 4/13
* 2/13
* 19/32

**5. Principal Component Analysis (PCA)**
Which of the following statements is true about PCA?
i) We must standardize the data before applying.
ii) We should select the principal components which explain the highest variance.
iii) We should select the principal components which explain the lowest variance.
iv) We can use PCA for visualizing the data in lower dimensions.
* (i), (ii), and (iv)
* (ii) and (iv)
* (iii) and (iv)
* (i) and (iii)

**6. System of Equations**
Determine the exact number of solutions for the following system:
$$2x + y - z = 1$$
$$x - 2y + z = -2$$
$$-x + 2y - z = -1$$
* 0
* 1
* Infinite
* Cannot be determined

**7. Neural Networks**
A 3-input neuron has weights 1, 4, and 3. The transfer function is linear with the constant of proportionality being equal to 3. The inputs are 4, 8, and 5 respectively. What will be the output?
* 51
* 153
* 54
* 160

**8. Medical Screening Statistics**
In a medical testing scenario, avoiding false negatives (Type II error) is strictly prioritized over false positives (Type I error) to prevent missing a diagnosis. How must the target p-value threshold be adjusted to satisfy this constraint?
* We would choose a higher p-value
* We would choose a lower p-value
* We would choose the same p-value
* False negatives do not depend on p-value

**9. Logistic Classification**
When classifying data with logistic classification, what is the upper bound of the likelihood in the maximum likelihood method? Is this value attainable?
* 1, Yes
* $e$, No
* 1, No
* 0, Yes

**10. Statistical Estimators**
Let $M$ and $S^2$ be the mean and variance of a random sample of size $> 1$ respectively from a normal population with an unknown mean $\mu$ and unknown finite variance $\sigma^2 > 0$. Consider the following statements:
1) $S^2$ is an unbiased estimator of $\sigma^2$, and $S$ is an unbiased estimator of $\sigma$.
2) $\frac{n-1}{n}M$ is an unbiased estimator of $\mu$, and $\frac{n-1}{n}S^2$ is an unbiased estimator of $\sigma^2$.
Which of the following statements is/are true?
* 1 only
* 2 only
* Both 1 and 2
* Neither 1 nor 2

**11. Matrix Rank Bounds**
If $\text{rank}(A) = 2$ and $\text{rank}(AB) = 3$, define the mathematical bound or exact value required for $\text{rank}(B)$.
* $\text{rank}(B) = 3$
* $\text{rank}(B) \leq 3$
* $\text{rank}(B) \geq 3$
* Data insufficient

**12. Infinite Solutions**
The following set of equations has infinite solutions, if $a = ?$
$$x + y + z = 1$$
$$ax - ay + 3z = 5$$
$$5x - 3y + az = 6$$
* -3
* 3
* -4
* 4

**13. Linear Regression**
Suppose you have a dataset with $m=50$ examples and $n=200,000$ features for each example. You want to use multivariate linear regression to fit the parameters $\Theta$ to your data. Should you prefer gradient descent or the normal equation?
* Gradient descent, since inverse $(X^T X)^{-1}$ will be very slow to compute in the normal equation.
* Gradient descent, since it will always converge to the optimal $\Theta$.
* The normal equation, since it provides an efficient way to directly find the solution.
* The normal equation, since gradient descent might be unable to find the optimal $\Theta$.

**14. Eigenvalues**
The eigenvalues of a 4x4 square matrix having 0's as the diagonal elements and 1's on the off-diagonal elements is:
* 2, -2, 0, 0
* 1, -1, 1, -1
* 3, -1, -1, -1
* 4, 0, 0, 0

**15. Matrix Powers**
Let $A$ be the 2x2 matrix with elements $a_{11} = a_{12} = a_{21} = 1$ and $a_{22} = -1$. Then the eigenvalues of the matrix $A^{19}$ are:
* $1024$ and $-1024$
* $1024\sqrt{2}$ and $-1024\sqrt{2}$
* $4\sqrt{2}$ and $-4\sqrt{2}$
* $512\sqrt{2}$ and $-512\sqrt{2}$

**16. Calculus Derivative**
Given $y = x^x$, what is $\frac{dy}{dx}$ at $x = 2$?
* $4(1+\log 2)$
* $4(2+\log 2)$
* 4
* 8

**17. Characteristic Equation**
If the characteristic equation of a matrix $A$ is $t^2 - t - 1 = 0$ then:
* $A^{-1}$ does not exist
* $A^{-1}$ exists but cannot be determined from the data
* $A^{-1} = A - I$
* $A^{-1} = A + I$

**18. Bias-Variance Tradeoff**
Data is sampled from a cubic function corrupted by Gaussian noise. You fit a linear model ($M_1$) and a 5th-degree polynomial model ($M_5$). Compare the expected bias and variance characteristics between $M_1$ and $M_5$.
* $\text{Bias}(M_1) \leq \text{Bias}(M_5)$, $\text{Variance}(M_1) \leq \text{Variance}(M_5)$
* $\text{Bias}(M_1) \geq \text{Bias}(M_5)$, $\text{Variance}(M_1) \leq \text{Variance}(M_5)$
* $\text{Bias}(M_1) \leq \text{Bias}(M_5)$, $\text{Variance}(M_1) \geq \text{Variance}(M_5)$
* $\text{Bias}(M_1) \geq \text{Bias}(M_5)$, $\text{Variance}(M_1) \geq \text{Variance}(M_5)$

<br><br>

## Part B: Programming Questions
<p><i>Data Structures, Algorithms, and Dynamic Programming. Use the provided LeetCode links for practical implementation.</i></p>

<br>

### 1. Find Median from Data Stream
**Difficulty:** Hard  
**Practice Link:** <a href="https://leetcode.com/problems/find-median-from-data-stream/description/" target="_blank">LeetCode - Find Median from Data Stream</a>

The median is the middle value in an ordered integer list. If the size of the list is even, there is no middle value, and the median is the mean of the two middle values.
* For example, for `arr = [2,3,4]`, the median is `3`.
* For example, for `arr = [2,3]`, the median is `(2 + 3) / 2 = 2.5`.

Implement the `MedianFinder` class:
* `MedianFinder()` initializes the MedianFinder object.
* `void addNum(int num)` adds the integer `num` from the data stream to the data structure.
* `double findMedian()` returns the median of all elements so far. Answers within $10^{-5}$ of the actual answer will be accepted.

> **Input:** > `["MedianFinder", "addNum", "addNum", "findMedian", "addNum", "findMedian"]`
> `[[], [1], [2], [], [3], []]`
> 
> **Output:** > `[null, null, null, 1.5, null, 2.0]`

**Explanation:**  
> `MedianFinder medianFinder = new MedianFinder();`  
> `medianFinder.addNum(1);    // arr = [1]`  
> `medianFinder.addNum(2);    // arr = [1, 2]`  
> `medianFinder.findMedian(); // return 1.5 (i.e., (1 + 2) / 2)`  
> `medianFinder.addNum(3);    // arr = [1, 2, 3]`  
> `medianFinder.findMedian(); // return 2.0`

<details>
<summary><b>View Constraints</b></summary>
<ul>
  <li>$-10^5 \leq \text{num} \leq 10^5$</li>
  <li>There will be at least one element in the data structure before calling <code>findMedian</code>.</li>
  <li>At most $5 \times 10^4$ calls will be made to <code>addNum</code> and <code>findMedian</code>.</li>
</ul>
</details>

<br>

### 2. Non-overlapping Intervals
**Difficulty:** Medium  
**Practice Link:** <a href="https://leetcode.com/problems/non-overlapping-intervals/description/" target="_blank">LeetCode - Non-overlapping Intervals</a>

Given an array of intervals `intervals` where `intervals[i] = [starti, endi]`, return the minimum number of intervals you need to remove to make the rest of the intervals non-overlapping. Note that intervals which only touch at a point are non-overlapping. For example, `[1, 2]` and `[2, 3]` are non-overlapping.

**Example 1:**
> **Input:** > `intervals = [[1,2],[2,3],[3,4],[1,3]]`
> 
> **Output:** > `1`
> 
> **Explanation:** > `[1,3]` can be removed and the rest of the intervals are non-overlapping.

**Example 2:**
> **Input:** > `intervals = [[1,2],[1,2],[1,2]]`
> 
> **Output:** > `2`
> 
> **Explanation:** > You need to remove two `[1,2]` elements to make the rest of the intervals non-overlapping.

**Example 3:**
> **Input:** > `intervals = [[1,2],[2,3]]`
> 
> **Output:** > `0`
> 
> **Explanation:** > You don't need to remove any of the intervals since they're already non-overlapping.

<details>
<summary><b>View Constraints</b></summary>
<ul>
  <li>$1 \leq \text{intervals.length} \leq 10^5$</li>
  <li>$\text{intervals}[i]\text{.length} == 2$</li>
  <li>$-5 \times 10^4 \leq \text{start}_i < \text{end}_i \leq 5 \times 10^4$</li>
</ul>
</details>

<br>

### 3. Minimum Cost to Reach Destination (Dynamic Programming)
An environment consists of `N` cities. You start at city `1` and must reach city `N`. From any city `i`, you can travel to city `i+1` or city `i+3` (if they exist within bounds). You are given an array `Cost` representing city tariffs. The price of traveling between city `i` and `j` is calculated as `|Cost[i] - Cost[j]|`. 

Your task is to find and return the minimum possible accumulated cost of a flight ticket required to reach city `N`.

**Note:** The number of cities is always greater than 3. Assume 1-based indexing.

**Example 1:**
> **Input:** > `N = 4, Cost = [1, 4, 5, 2]`
> 
> **Output:** > `1`
> 
> **Explanation:** > Travel optimally from city 1 to city 4 directly (city 4 is the third next city). The cost is `|1 - 2| = 1`.

**Example 2:**
> **Input:** > `N = 6, Cost = [4, 12, 13, 18, 10, 12]`
> 
> **Output:** > `10`

**Explanation:**  
> Travel optimally from city 1 -> 2 -> 3 -> 6.  
> Cost 1 to 2 = `|4 - 12| = 8`  
> Cost 2 to 3 = `|12 - 13| = 1`  
> Cost 3 to 6 = `|13 - 12| = 1`  
> Total accumulated cost = `8 + 1 + 1 = 10`

<p align="center">
  ~~~~~···~~~~~···~~~~~·····~~~~~···~~~~~···~~~~~  
</p>

<p align="center">
  ⭐ If this project helped you, please <a href="https://github.com/cu-sanjay/Amazon-ML-Summer-School-2026">star the repository</a> ⭐
</p>
