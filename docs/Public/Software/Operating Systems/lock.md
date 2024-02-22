A *lock* is a [[synchronization variable]] that provides mutual exclusion; a [[thread]] will be guaranteed to proceed.

There are two states: `locked` and `free`

For example, a *lock* can stop an [[interrupt]] from preemptively ([[preemption]]) stopping a thread. 
