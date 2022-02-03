Start a new session with session name
```
screen -S <session_name>
```

Detach
```
ctrl+a d
```

Search a string in the screen session:
```
ctrl+a esc ?  (3 steps)
<type seach string>
n to move next instance in up side
shift+n to move next instance in down side
```


Kill particular window in screen session
```
ctrl+a k (then press 'y' to confirm)
```

kill the screen session

```
// Find the pid of screen session using 'screen -ls' command
screen -S <PID> -X quit
```

Increse scroll back buffer size in screen
```
// Add below line in ~/.screenrc
defscrollback 100000
// (or)
ctrl+a :scrollback 10000
```

Start and Stop recording screen logs
```
ctrl+a H
```

Re-attach to the screen
```
screen -r
```

Fixing "There is no screen to be resumed." issue while re-attach
```
screen -d -r <pid>
```
