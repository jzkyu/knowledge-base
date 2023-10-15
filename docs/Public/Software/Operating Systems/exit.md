An *exit* occurs when the command finishes. 

A `0` indicates success. Any other value indicates error. 

```bash
echo "Hello" > /dev/null
echo $?
0

cat missing.txt
cat: missing.txt: No such file or directory
echo $?
1
```