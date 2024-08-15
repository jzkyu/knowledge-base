See: [[one hot decoder]]

A *one hot encoder* has one [[flip flop]] per state, and exactly one of these flip flops will be $1$ at a time. 

Another way to think of it, is that you have a [[binary]] [[vector]] of length $n$, where the vector is all zeroes except for the index that corresponds to the category, which is set to $1$.

For the three categories, "Red", "Green", and "Blue":
- "Red": [1, 0, 0]
- "Green": [0, 1, 0]
- "Blue": [0, 0, 1]

