*See: * [[stream]]

A *redirection* is a way to change the standard input / output of the [[CLI]] to point to and from files. [^1]
You can redirect `stdout` to a file like this:
```bash
echo "Hello World!" > hello.txt
cat hello.txt
```

Redirect `stdin`: 
```bash
cat < hello.txt
```

Append `stdout` to a file:
```bash
cat < hello.text >> hello_copy.txt
```


[^1]: https://www.guru99.com/linux-redirection.html