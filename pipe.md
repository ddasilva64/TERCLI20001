# Pipe



It is used to chain the standard output of a command with the standard input of another command. For this you use |.

```
| wc -l         -> shows number of output lines
```

```bash
$ ls -l | wc -l
```

```
| grep [pattern] -> returns the lines that meet the pattern
```

```bash
$ cat movies.csv | grep thriller
```

```
| more           -> show the list of results by pages
```

```bash
$ cat movies.csv | more
```
