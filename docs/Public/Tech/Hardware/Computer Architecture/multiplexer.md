A *multiplexer* selects one of its [[data]] ports to forward to the output based on the selection signal.

It behaves like a switch statement in programming. 

![[Mux.png]]

In general, a *multiplexer* has $2^n$ data inputs and requires $n$ select bits to choose which one will be the output. Larger *multiplexers* can be constructed with [[gate]] and [[tree]] of other *multiplexers*. 