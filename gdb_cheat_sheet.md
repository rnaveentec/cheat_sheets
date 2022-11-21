
Attach GDB to a running process

```
bash#gdb /pid <pid_of_process>
```

Get backtrace from all the thread of a process
```
(gdb)thread apply all bt
```

List all the threads of a process
```
(gdb)info thread
```

Switch to a particular thread.(get the thread number from "info thread")
```
(gdb)thread <thread_number>
```

apply break point only for a particular thread
```
(gdb) break <funcion_name> thread <#thread_id>
```

Attach GDB. Print the bt and detach

```
bash# gdb -batch -ex bt –p <pid>
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
(gdb)end 
```

How to set number of elements to print from the array?
```
set print element <number of element>
```

How to print complete content of the array in GDB?
```
set print element 0
```

How to save breakpoint to a file?
```
save breakpoints filex.brk
```

How to load break points from a file?
```
set breakpoint pending on
source filex.brk
```

How to avoid pressing next/enter repeatedly in large functions ?
```
(gdb) define nnext
> set $foo = $arg0
> while ($foo--)
 >  next
 >  end
> end
(gdb) nnext 100
```
