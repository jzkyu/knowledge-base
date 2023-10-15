A *path* is a special variable used to find the executable of a program. The [[shell]] searches `$PATH` when you enter a [[command]]. 

```bash
which ls
/usr/bin/ls
echo $PATH
/usr/local/sbin:/usr/local/bin:/usr/bin:/opt/cuda-10.1/bin:/usr/lib/jvm/default/bin ...
echo $PATH | sed 's/:/\n/g'
/usr/local/sbin
/usr/local/bin
/usr/bin
/opt/cuda-10.1/bin
/usr/lib/jvm/default/bin
```
- You can run a program without searching for its path
```bash
./hello
Hello World!
```

```bash
hello
bash: hello: command not found
sudo mv hello/usr/local/bin
hello
Hello World!
```