A *non-deterministic finite automata*, or *NFA*, is a [[DFA]] with the following differences:
- An *NFA* state may have any number (including $0$) of transition arrows out of a [[state]], for the same input [[symbol]]. 
- An *NFA* may change states without reading any input (an $\epsilon$-transition)
- If there is a series of choices (when there is a choice) to reach an accept state after reading the whole [[string]], than the *NFA* accepts. Otherwise, the *NFA* rejects.

