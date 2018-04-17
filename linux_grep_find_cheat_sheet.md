Find all the executable recursively
```
find . -type f -executable
```
Find and delete all the executable recursively 
```
find . -type f -executable | xargs rm
```
