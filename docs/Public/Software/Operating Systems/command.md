A *command* is a request to perform an operation or run a program. 

You can add a [[flag]] which affect how a *command* can work. 

`;`:
- Execute *commands* in series
```bash
echo -n "hello " ; echo "world"
hello world
```

`&&`:
- Conditionally on success
```bash
cat / && echo "world"
cat: /: Is a directory
cd ~/slides/ && du -sh Makefile
4.0K  Makefile
```

`||`:
- Conditionally on failure
```bash
cat / || echo "Cat failed"
cat /: Is a directory
Cat failed
echo -n "hello" || echo "world"
hello
```