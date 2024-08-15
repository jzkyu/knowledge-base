A *Turing machine* is a [[finite state machine]] with an unbounded read / write tape.  

There are some key difference compared to a FSM:
- When writing, it can write more than just what the input [[alphabet]] allows.
- The tape head (pointing to a character in the input) can move left or right. 
- There is one accept and reject state, that halts the machine.

Example for $P = \{ w\in \{0, 1\}^* |  w = w^2 \}$:

![turing](turing.png)