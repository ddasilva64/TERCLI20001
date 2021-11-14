# Find files



```
find <directory> -name [name] -> search based on the name and metadata within the directory that we tell it
-name                         -> the filename (* .js returns all files ending with .js)
-type                         -> the type
```

`find source_directory -type f -name [name] -exec [action] {} ./destination_directory \;` -> searches files according to search criteria and copies or moves them all to a specified directory

* \-action -> can be `mv` to move or `cp` to copy

**Note:** set the -type f attribute to select only files and put ; to end the command
