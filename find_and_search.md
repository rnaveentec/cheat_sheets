
## Find command for files

1. Find a file from home/any folder recursively 

    ```find . -name -type d -name <file name>```

2. Search the file only to the next level folder(**maxdepth used for it**)

    ```find -maxdepth 2 -type f -name <file name>```   

3. Find all the executable recursively

    ```find . -type f -executable```

4. Find and delete all the executable recursively

    ```find . -type f -executable | xargs rm```



## Find command for directory

5. Get specifc fields from 'ls -l' output
   ```ls -l *test | cut -d " " -f 9```
   Above command list all the file names ends with test(XXXXXtest) and the cut command with -d(delimiter) -f(filed) options print the nineth field sperated by space.
