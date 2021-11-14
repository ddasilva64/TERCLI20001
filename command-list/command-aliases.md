# Command aliases



```
alias [command_alias]='[command]' -> create an alias for a defined command
```

```bash
$ alias ll='ls -lh'
```

In this example the command is being created `ll` what will execute `ls -lh`

Anything added after the alias is automatically added after the command

```bash
$ ll -a
$ ls -lh -a
```

In the example, 2 commands do the same

Every time we open the terminal a program called `.bash_profile` which is a series of commands that register some variables

In `.bash_profile` aliases are saved
