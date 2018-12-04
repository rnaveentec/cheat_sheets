## How to install tmux?

```sudo apt-get install tmux```

## How to start tmux?

We can start tmux with/without session name
1. Without a session name

```
tmux
```
2. With Session name

```
tmux new -s <Session name>
```

## How to detach from tmux session?

```
"Ctrl + b" then d
````

## How to attach to tmux session?

```
tmux a
```

## How to attach tmux to a named session?

```
tmux a -t <Session name>
```
# New window

## How to create new window?

```
"Ctrl+b" then c
```

## How to switch window

```
"Ctrl+b" then <window number>
```

(Or)
To list all the window and select particular window.
```
"Ctrl+b" then w
```
Now select the window


# Split pane

## Vertical split
```
"Ctrl+b" then %
```

## Horizontal split

```
"Ctrl+b" then "
```

## How to switch pane?

```
"Ctrl+b" then Arrow key
```

## How to kill pane?

```
"Ctrl+b" then x
```
