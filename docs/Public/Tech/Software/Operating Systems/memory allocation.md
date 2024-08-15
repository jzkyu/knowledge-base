*Memory allocation* is creating space in a spot of [[memory]] where [[data]] can be stored.

When declaring static or global variables, *static allocation* creates a block of space, a fixed size of the variable, and is never freed. [^1]

In cases where the size of the data structure is not known before the program runs, you would want to do *dynamic memory allocation*. In other words, the size of the data structure is changed during [[runtime]]. [^2]

[^1]: https://www.gnu.org/software/libc/manual/html_node/Memory-Allocation-and-C.html
[^2]: https://www.geeksforgeeks.org/dynamic-memory-allocation-in-c-using-malloc-calloc-free-and-realloc/