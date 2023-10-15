A *pipe* is used to combine two or more commands. It will take the output of a [[command]] and use that as the input for the next command. [^1]

Using the *pipe* '|' character: 
```bash
ls -l / | tail -n3
```

You can chain *pipes* together. 

[^1]: https://www.redhat.com/sysadmin/pipes-command-line-linux