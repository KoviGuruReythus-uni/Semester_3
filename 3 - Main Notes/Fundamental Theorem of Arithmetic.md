
2026-09-09
07:09
share: true
Tags: [NumberTheory](NumberTheory) 
___
# Fundamental Theorem of Arithmetic
Every int other than 0 and $\pm 1$ can be represented as a product of primes.
This representation is unique _up to_ the order and sign of the factors
	_this simply means that the order and sign are NOT unique_
___
## Proof of Existence of Factorisation
### Initial State
$n \in \mathbb{Z}$ 
$|n| > 1$

The first factor is $n$ itself.

### Base Case
Evaluate a sequence of factors. 
$a_1, a_2...a_k$ where all $a_i$ are primes

If this condition (all the numbers $a_i$ are primes) is met, the algorithm stops. (if not, we continue onto the iterative step) 

### Iterative Step
If at least one of the factors $a_i$ is composite, 
	this means that $a_i$ can be written as a product of primes $b,c$ 
		where $|b|, |c| > 1$ _(this stops the algorithm from running infinitely by considering $b=1, c=a_i$ or vice versa)_ 

If such a composite number if found, we replace $a_i$ with $b,c$ 

### Proving algorithm termination
_we must prove that the sequence of factors cannot grow infinitely_
- Every time the algorithms runs, one factor (composite number) is destroyed and in place, there are 2 factors. 
	- The total number of factors ($k$) increases by 1 per iteration
- The smallest number of factors is 2

And since $|b|, |c| > 1$, the smallest absolute value of the factors is 2
$$
\begin{align}
Since, \\
|n| &= |a_1|.|a_2|...|a_k| \\
And\ the\ smallest\ &absolute\ value\ of\ the\ factors\ is\ 2, \\
|n| &\geq 2.2...2\ (multiplied\ k\ times) \\
|n| &\geq 2^k \\
\implies log_2(|n|) &\geq k \\
\implies k &\leq log_2(|n|)
\end{align}
$$

This proves that there is a finite upper limit $log_2(|n|)$ for $k$ and that it cannot go on till infinity.
___
## Proposition
Let's assume $p_1,...,p_k$ are pairwise different positive primes
	$n = p_1^{\alpha_1}...p_k^{\alpha_k}$ 
		where, $\alpha_1,...,\alpha_k$  are non-negative integers

Then, some positive integer $m$ divides $n$ iff 
	$m=p_1^{\beta_1}...p_2^{\beta_k}$ 
		where, $0 \leq \beta_1 \leq \alpha_1,..., 0 \leq \beta_k \leq \alpha_k$ 
			_also $\beta_i$ are all ints_ 

### Plain English
For an int m to be able to divide some other int n, all the powers of the prime factors of m must be less than or equal to those of n. 

Eg: $4|204 \implies 2^2|(2^2 . 3^1 . 17^1)$ 