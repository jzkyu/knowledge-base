*See:* [[stream]]
`head`:
- Sends the first `n` lines of its input to its output
```bash
head -n3
```

`tail`: 
- Sends the last `n` lines of its input to its output
```bash
tail -n3
```

```bash
ls -l / > temp.txt
tail -n3 < temp.txt
```

`grep`: 
- Searches the input stream for a string
- Outputs every line that contains the string
```bash
history | grep tail
```

`cut`:
- Removes sections from each line of the input
- Useful when filtering columns from input
```bash
cat foo.txt
A,B,C,D
A,B,C,D
B,B,C,D
D,C,B,A
cat foo.txt | cut -d "," -f1,4
A,D
B,D
D,A
```

`sort`:
- Sorts the input and sends it to `stdout`
- Defaults to alphanumeric sort, but it has many sorting options

`uniq`:
- Outputs the unique lines in the input
- Only detects repeated lines if they are adjacent
	- Input needs to be sorted first
```bash
sort foo.txt | uniq     // Display each line once
sort foo.txt | uniq -u  // Display only unique lines
sort foo.txt | uniq -d  // Display only duplicated lines
sort foo.txt | uniq -c  // Display frequency of each line
```

`tee`:
- Read from standard input and write to standard output and files
```bash
echo 1 | sudo tee /sys/class/leds/input2::scrolllock/brightness
```


