
## Install Cscope and Ctags

```
sudo apt-get install cscope
sudo apt-get install ctags
```
   
## One-Liner to Build cscope and ctags for .c and .cpp files

```
find . -name '*.c' -o -name '*.cpp' -o -name '*.h' > cscope.files && /usr/bin/ctags -L cscope.files && cscope -b"
```

## Cscope Alias 

You can add the commad as alias in ~/.bashrc file to build the cscope. *cd* inside specific folder and run *bldcscope* command.
   
```
alias bldcscope="find . -name '*.c' -o -name '*.cpp' -o -name '*.h' > cscope.files && /usr/bin/ctags -L cscope.files && cscope -b"
```

## Start cscope

```
cscope
```

## Short Cut keys to brows the code
1. Jump in to the definition

```ctrl + ]```

2. Jump back to the previos place where we used **ctrl+ ]**

```ctrl + t```

3. Move to starting of the function

```[[```

4. Move to end of the function

```]]```

5. Move to matching close/open for any of these 6 charecter **[{()}]**

```%```

## Exit from cscope

```ctrl + d```
