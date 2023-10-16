*See:* [[minterm]]

A *maxterm* is a sum of all [[literal]] values in a function. 

If the literal is 1, it will be the complementary form of the variable ($\neg A$)
If the literal is $0$, it will be the positive form of the literal ($A$)

For example, for the function $f$ with inputs $A$, $B$, and $C$:
- Is a maxterm: $A+\neg B+\neg C$
- Is not a maxterm: $A+B$

To find the POS:
- Select the rows that are false and [[and]] the corresponding *maxterms*