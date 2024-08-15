*SSH* (Secure SHell) is a [[network]] [[protocol]] that enables two computers to communicate and share data securely over insecure networks through encrypted connections. [^1]

*SSH* is often used to "login" and perform operations on remote computers, but can also be used for transferring data. [^1]

Basic commands:
```bash
ssh <user>@pc<#>.cs.ucdavis.edu
```

You can run a [[command]] on remote machines and [[pipe]] the result:
```bash
ssh noah@pc17.cs.ucdavis.edu ls | grep Downloads
```

[^1]: https://www.ucl.ac.uk/isd/what-ssh-and-how-do-i-use-it