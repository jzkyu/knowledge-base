*See:* [[maxterm]]

A *minterm* is a [[product]] of all [[literal]] values in a function. 

If the literal is $1$, it will be the positive form of the literal ($A$)
If the literal is $0$, it will be the complementary form of the literal ($\neg A$)

For example, for the function $f$ with inputs $A$, $B$, and $C$:
- Is a maxterm: $\neg ABC$
- Is not a maxterm: $A\neg B$

To find the SOP:
- Select the rows of output that are True and [[or]] the corresponding *minterms*