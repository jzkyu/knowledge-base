A *process* is a program or [[command]] that is actually running on the computer. [^1]
The [[operating system]] can run many different processes at the same time. [^1]

![process.png](process.png)

*Process* commands on the [[CLI]]:

`Ctrl+C`:
- Stops a process
```bash
sleep 60
^C
```

`Ctrl+Z`:
- Pause a process
```bash
sleep 5
^Z
[1]+ Stopped          sleep 5
echo "Hello"
Hello
```

`fg`, `bg`:
- Resume in either foreground or background
```bash
fg
sleep 5
```

```bash
bg
[1]+ sleep 5 &
echo "What now?"
What now?
[1]+   Done           sleep 5
```

`&`:
- Start a process in the background
```bash
cat /dev/random > /dev/null &
```

`jobs`:
- Lists all jobs (processes)
```bash
jobs
[1]-   Stopped                   cat /dev/random > /dev/null
[2]+   Stopped                   sleep 10
```

`kill`:
- Terminate jobs (processes)
```bash
kill %1
[1]+   Terminated                cat /dev/random > /dev/null
```

- Jobs are tied to the [[terminal]] session
	- Exiting terminal kills stopped and backgrounded jobs

- Protect background job from terminal exit:
```bash
nohup sleep 10 &           // "no hang up" for a new job
disown %1                  // For a job already running
```

[^1]: https://www.ibm.com/docs/pt-br/aix/7.1?topic=administration-commands-processes