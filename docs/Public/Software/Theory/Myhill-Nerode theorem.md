The *Myhill-Nerode theorem* is used to prove whether a language is regular or not. 

For any [[language]] $L\in \Sigma^*$, say two strings ([[string]]) $x, y \in \Sigma^*$ have a separating (distinguishing) extension $z\in \Sigma^*$ if $xz\in L \iff yz \not \in L$. (Exactly one of $xz$ or $yz$ is in $L$). In this case, we say $x$ and $y$ are *L-separable*. 
- It's okay if one of them is in $L$, if the other one is not in $L$
- $xz \not \in L \iff yz \not \in L$ also holds true

We say $x$ and $y$ are *L-equivalent*, written $x \sim y$ if they are not *L-separable*, i.e. for all $z\in \Sigma^*$, $xz\in L \iff yz \in L$. 

A language $L$ is a [[regular language]] if and only if $\sim_L$ defines a finite number of equivalence classes. Furthermore, the number of equivalence classes of $\sim_L$ equals the number of states in the smallest [[DFA]] that decides. 

Corollary - For a language $L$, if $\sim_L$ defines an infinite number of equivalence classes, then $L$ is not a [[regular language]]. 
