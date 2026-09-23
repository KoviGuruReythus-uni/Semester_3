08-Sep-26
05:30

Tags:  [Probability](Probability.md)
___
# Sample Space
$\ohm$ is an arbitrary set
1. SAMPLE SPACE: $\ohm$
2. OUTCOME: an element $\omega \in \ohm$
3. EVENTS: selected subsets $A \subseteq \ohm$
4. PROBABILITY: a number $P(A) \in [0,1]$ assigned to an event $A$ 

Events are _SELECTED_ subsets - We only consider the subsets (from $\ohm$) that are of interest to us, that we want to find the probability of. And we call those specific subsets _events._ 

## Operations on Events
1. $A \backslash B$ = $A \cap \bar B$
2. If $A \cap B = \phi$, $A,\ B$ are disjoint
3. Certain Event: $\ohm$ : $P(A)=1$
4. Impossible Event: $\phi$ : $P(A) = 0$
### DeMorgan's Laws
5. $\overline{A \cup B} = \bar A \cap \bar B$ 
6. $\overline{A \cap B} = \bar A \cup \bar B$
7. $\overline{\bigcup_{i=1} ^{\infty} A_i} = \bigcap_{i=1} ^{\infty} \overline{A_i}$ 
8. $\overline{\bigcap_{i=1} ^{\infty}A_i} = \bigcup_{i=1} ^{\infty} \overline{A_i}$ 

```tikz
\begin{document}
\begin{tikzpicture}
\draw (0,0) circle (1.3);
\draw (1.5,0) circle (1.3);
\draw (-2,-1.8) rectangle (3.5,1.8);
\node at (-0.7,1) {$A$};
\node at (2.2,1) {$B$};
\end{tikzpicture}
\end{document}
```
