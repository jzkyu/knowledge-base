*GDB* stands for the [[GNU]] debugger, which helps finds errors like segmentation faults. 

Canonical complication command line: 
```bash
gcc [cflags] -o <output> <input
``` 

Optimize for speed: (-O2)

```bash
gcc -Wall -Werror -O2 -o myprogram main.c
```

Enable debugging support (-g):
```bash
gcc -Wall -Error -g myprogram main.c
```
- To balance performance with debugging experience use `-Og`
- Not recommended to use debugging along with other optimizations
	- No optimization option is equivalent to `-O8`

Start GDB with the program to debug as an argument:
```bash
gdb myprogram
```

Running the program:
- Without any argument: `gdb run`
- With arguments: `gdb run argv1, argv2... `

GDB offers an interactive shell:
- Can ask `gdb help <argument>`

Possible scenarios:
1. Program doesn't have bugs
2. Best-case scenario: Segmentation fault
3. Worst-case scenario: Doesn't crash, but wrong output

Backtrace:
- First thing to do when getting a segfault
	- Understand what is the sequence of calls that brought us there
```bash
gdb backtrace
```
Breakpoints:
- Stop the program during the execution at a designated point
- At a line:
```bash
gdb break string-test.c.:13
Breakpoint 1 at 0x4005ef: file string-test.c, line 13.
```
- At a function:
```bash
gdb b main
Breakpoint 1 at 0x40059f: file string-test.c, line 8
```
- At a condition:
```bash
gdb b string-test.c:13 if i == 5
```
- Show info of all declared breakpoints:
```
gdb info b
```

Dealing with Breakpoints:
- Once the program has stopped and the gdb shell is available, you can:
	1. Continue the execution until the next breakpoint: `gdb continue` or `gdb c`
	2. Execute only the next line of code and break again: `gdb step` or `gdb s`
	3. Jump over function calls: `gdb next` or `gdb n`
- Tip: Typing `<enter>` in the interactive gdb shell repeats the last command




