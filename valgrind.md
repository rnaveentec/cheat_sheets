
1. If possible Compile code with -ggdb3 option


2. Start your program with valgrind
```
valgrind --leak-check=full --show-leak-kinds=all --track-origins=yes --verbose --log-file=valgrind-out.txt ./executable exampleParam1
```
  Valgrind Options Description:
  ```
    --leak-check=full: "each individual leak will be shown in detail"
    --show-leak-kinds=all: Show all of "definite, indirect, possible, reachable" leak kinds in the "full" report.
    --track-origins=yes: Favor useful output over speed. This tracks the origins of uninitialized values, which could be very useful for memory errors. Consider turning off if Valgrind is unacceptably slow.
    --verbose: Can tell you about unusual behavior of your program. Repeat for more verbosity.
    --log-file: Write to a file. Useful when output exceeds terminal space.
  ```

3. Check the valgrind-out.txt for the leak infp
