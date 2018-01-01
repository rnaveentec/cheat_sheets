
Attach GDB to a running process

```
gdb /pid <pid_of_process>
```

Attach GDB. Print the bt and detach

```
gdb -batch -ex bt –p <pid>
```

How to print a variable value each time when we hit a breakpoint?

```
(gdb)break <line>
Breakpoint <break-point-number> at <some XYZ address>
(gdb)command
Type commands for break point(s)<break-point-number>, One per line.
End with a line saying just "end".
>silent
>print <some variable>
>printf "x is %d\n",x
>continue 
>end
(gdb) set logging file gdb.txt
(gdb) set logging on
Copying output to gdb.txt.
(gdb) set pagination off
(gdb)continue 
```