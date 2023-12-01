An *instruction* is the basic elementary operations that a [[CPU]] can perform. [^1]

There are different kinds of *instructions*:
- R-Type *Instructions*
	- Register *Instructions*
	- rd = rs funct rt
		- rd = destination
		- rs = source
		- rt = target
		- funct = the bits of the instruction to perform
- I-Type *Instructions*
	- Immediate *Instruction*
	- rt = rs op Sign Extended Immediate
	- SEI means prepending the most significant bit of the immediate to the immediate until it is 32 bits big
- J-Type *Instructions*
	- Jump *Instructions*
	- PC = (PC+4)_{31:28}:addr:00, where ':' means concatenate
	- PC = program counter; the address of the *instruction* that we are currently working on right now

[^1]: https://www.geeksforgeeks.org/computer-organization-basic-computer-instructions/