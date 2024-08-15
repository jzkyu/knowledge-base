A *cache* is a temporary [[data]] store that holds data so future requests for that data can be serve faster. 

It is a smaller, faster memory component inserted between the main memory and the [[CPU]] that stores values recently accessed in [[memory]].

Requests to memory are intercepted to the cache:
1. If the cache has it, it serves it immediately
2. If the cache doesn't have it, it will make a request to memory and store the result for later

The *cache* can be extended beyond the original use:
- Main memory serves as a *cache* to the hard drive
- Registers serve as a *cache* for the *cache*

*Cache* is used for the internet a lot.

Terminology:
- Word: An element in memory
	- The unit of transfer between the *cache* and the CPU
- Block. A contiguous chunk (next to each other) of words in memory
	- Unit of transfer between memory and the *cache*
- Way: A Block inside of a set along with the additional overhead bits related to a block to make the *cache* work
- Set: a collection of Ways
- Cache: a collection of Sets
