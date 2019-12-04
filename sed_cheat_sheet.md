delete 10th line from a  file

```
sed -i '10d' <file>
```

Replace a word in a particular line
> Below command will replace the word "bad" with "good" on line number 2 in hello.txt file.

```
sed -i '2s/bad/good/' hello.txt
```

Delete Trailing white spaces in python file
```
sed --in-place 's/[[:space:]]\+$//' file_name
```
