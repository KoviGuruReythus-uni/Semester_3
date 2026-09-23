21-Sep-26
08:50

Tags: [Probability Space](Probability%20Space.md) 
___
# Probability Measure

Let $\digamma$ be $\sigma$ algebra over $\ohm$. 
The function $P : \digamma \to [0,1]$ is called probability measure if
	1.  $P(\ohm) = 1$ 
	2. $P( \bigcup_{i=1}^{ \infty} A_i) = \Sigma_{i=1} ^{\infty} P(A_i)$  for all $A_i \in \digamma$ that are _pairwise disjoint_ ie, $A_i \cap A_j = \phi$ whenever $i \neq j$ 
		_this property is called $\sigma$ additivity_
## Writing this in plain english now
What is a probability measure? 
1. It is a function
	$P: \digamma \to [0,1]$ 
		This means, the domain of $P$ is $\digamma$ and that it maps to numbers ranging from 0 up to and including 1. 
			$x$ - axis is $\digamma$ which means that there are all the possible events there
			$y$ - axis is $[0,1]$ 
		The graph will plot the probabilities of all the events in $\digamma$ which we defined earlier is also $\sigma$ algebra. _(look here for further explanation: [Event Algebra](Event%20Algebra.md) )_

2. There is also one more condition that it has to satisfy,
		for all pairwise disjoint events in $\digamma$, the probability of union of all of them is equal to the sum of probabilities of each of them individually. 

