## Indentation

### Kernighan & Ritchie style

```
indent -kr <.c file name>
```

### Static analysis

```
splint <.c  file name>
```

### Oneliner to host the directory
```
pushd test; python3 -m http.server 9999; popd;
```
