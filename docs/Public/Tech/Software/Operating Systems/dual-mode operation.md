*Dual-mode operation* makes a trade-off between a user mode and kernel mode when executing programs. 

There are distinct execution modes supported directly in hardware:
- In kernel mode, a process has full [[privilege]] with the hardware
- In user mode, a process has limited privilege on the hardware

What *dual-mode operation* provides for the hardware:
- Privileged instructions
	- Exception handler: will talk to kernel if a process has gone bad
- [[memory protection]]
- Timer interrupts
- Mode switch

