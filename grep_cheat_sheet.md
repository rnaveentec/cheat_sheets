1.Avoid grep error such as "Permission denied" "no such a file or directory"

```
grep "String" * -R -s -n
```

2. Grep based on file name

     a. With case sesitive
     
     ```
     grep -r --include=\*.txt 'searchterm' ./
     ```
     
     b. Ignore case sensitive
     
     ```
     grep -r -i --include=\*.txt 'searchterm' ./
     ```

    **Explanation**:
    
     grep: command
     
     -r: recursively
     
     -i: ignore-case
     
     --include: all *.txt: text files (escape with \ just in case you have a directory with asterisks in the filenames)
     
     'searchterm': What to search
     
     ./: Start at current directory.

