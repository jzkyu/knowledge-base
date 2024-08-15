An *adder* is a logic circuit that adds [[binary]] numbers. It takes an input of two bits, and outputs two bits in sum and carry terms. 

A half *adder* produces the sum of the two inputs as a sum bit and carry out bit. 

![[HalfAdder.png]]

| A | B | Sum | Carry Out |
| --- | --- | --- | --- |
| 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 0 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 1 |

A full *adder* also considers the carry input, the sum of three inputs as a sum bit and carry out bit. 

![[FullAdder.png]]

| Carry In | A | B | Sum | Carry Out |
| --- | --- | --- | --- | --- |
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 | 0 |
| 0 | 1 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 1 | 0 | 1 | 0 | 1 |
| 1 | 1 | 0 | 0 | 1 |
| 1 | 1 | 1 | 1 | 1 |

You can string multiple full *adders* together to create a ripple carry *adder*. The Carry Out bit of the previous *adder* stage will be the Carry In bit of the next *adder* stage.
- However, this method is slow - you have to wait for the carry to propagate all the way through to the last stage

![[RippleCarryAdder.PNG]]

To reduce the delay on the carry, we can calculate the carries in parallel. Distributing the terms is known as a prefix *adder*. 



