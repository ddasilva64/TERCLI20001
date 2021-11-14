# Files and directories manipulation



```
cat [file_name_1]  [file_name_2]                 -> concatenates the contents of first file and second fille to the terminal output
cd                                               -> changes to the user's home directory ($HOME)
cd <directory>                                   -> changes to the directory
cd ..                                            -> moves up one level in the directory tree structure
cd ../..                                         -> changes two level up directories from the current one
cp <origin_file> <destination_file>              -> copies a file into destination path file
cp -r <origin_directory> <destination_directory> -> recursively copies a directory and its contents into new one
file <file>                                      -> shows the file characteristics 
head [file_name]                                 -> shows the first 10 lines of a file
head -n 20 [file_name]                           -> shows the first 20 lines of a file
gpg [file_name.gpg]                              -> decrypt a file
gpg -c [file_name]                               -> encrypts a file
less [file_name]                                 -> explores file content with pagination
ln -s <file> [link_name]                         -> creates a symbolic link to a file
ls                                               -> lists files and directories
ls -a                                            -> lists all files, including hidden
mkdir <directory>                                -> creates a new directory
more [file_name]                                 -> shows the contents of a file
mv <file> <directory>                            -> moves a file into destination path
mv [file_name] [new_file_name]                   -> renames a file to new one
open <file>                                      -> opens a file with default program in macOS
pwd                                              -> shows the directory currently working in
rm <file>                                        -> removes a file
rm -r <directory>                                -> removes a directory and its contents recursively
rm -ri <directory>                               -> removes a directory and its contents interactively
rm -rf <directory>                               -> removes a directory recursively without requiring confirmation
tail [file_name]                                 -> shows the last 10 lines of a file
tail -n 20 [file_name]                           -> shows the last 20 lines of a file
touch <file>                                     -> creates a new empty file 
tree /path                                       -> shows all the files and subdirectories
tree -L 2 .                                      -> shows all the files and subdirectories with two levels deep
wc                                               -> prints the number of words, lines, and bytes in a file
xdg-open <file>                                  -> opens a file with the default program in the most Linux distros
```
