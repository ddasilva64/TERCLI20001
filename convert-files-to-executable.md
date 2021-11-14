# Convert files to executable



```
#! <executable directory> -> returns a file as executable, we are specifying who is going to execute the command that follows

#!                        -> it must necessarily be included at the beginning of the file. In the first line
```

```php
#! /usr/local/bin/php
<?php
date_default_timezone_set("America/Bogota");
printf("%s\n", data("Y-m-d H:i:s"));
```

In this case, we are indicating to `/usr/local/bin/php` to run the command that is on the subsequent lines

So when we run `example.php` it runs automatically and you no longer have to indicate who is going to do it
