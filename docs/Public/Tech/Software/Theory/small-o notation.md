*Small-o notation* represents the upper bound of the [[runtime]] of an [[algorithm]]; the runtime will be strictly smaller than *Small-o*. It gives the worst case complexity of an algorithm. [^1]

If $f = O(g)$ and $g \ne O(f)$, then
$$
f = o(g) \iff \lim_{n \to \infty} \frac{f(n)}{g(n)} = 0
$$
It can also be said that `f` is "strictly less than" $g$.

![[big_o.png]]

[^1]: https://www.programiz.com/dsa/asymptotic-notations