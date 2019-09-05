# Reference List

Also refer to [CS246](https://www.student.cs.uwaterloo.ca/~cs246/) course site for more resource

## Linux Shell

- General
  - Display command help
    ```shell
    man [command]
    ```
  - Clear the the screen
    ```shell
    clear
    ```
  - Input Redirection
    ```shell
    [command] < [file]
    ```
  - Output Redirection
    ```shell
    [command] > [file]
    ```
  - Shortcut  
    ```^L ``` for clear screen  
    ```^C``` for terminating program  
    ```^D``` for eol (End of Line) signal  
- Navigation
  - Navigate in to folder
    ```shell
    cd [path]
    cd ~
    cd ..
    ```
    `~` is used for going to root  
    `..` is for going up the directory tree (to parent folder)
  - Display files/directories in current directory  
    [manual](http://man.he.net/?topic=ls&section=all)
    ```shell
    ls [option]
    ```
    Some common options are  
    `-a` for all file (include hidden files)
  - Display path
    ```shell
    pwd
    ```
  - Read file  
    [manual](http://man.he.net/?topic=cat&section=all)
    ```shell
    cat [file]
    ```
  - Count  
    [manual](http://man.he.net/?topic=wc&section=all)
    ```shell
    wc [file]
    ```
    Some options are  
    `-c` print the byte count
    `-m` print the character count
    `-l` print the line count
    `-w` print the word count
<!-------------------------------------------------------------------------->
- File/Folder Manipulation
  - Create Directory  
    [manual](http://man.he.net/?topic=mkdir&section=all)
    ```shell
    mkdir [folder]
    ```
  - Remove Directory (if it's empty)
    [manual](http://man.he.net/?topic=rmdir&section=all)
    ```shell
    rmdir
    ```
  - Remove Directory (and all children)
    ```shell
    rm -r [folder]
    ```
  - Remove File  
    [manual](http://man.he.net/?topic=rm&section=all)
    ```shell
    rm [file]
    ```
  - Copy File  
    [manual](http://man.he.net/?topic=cp&section=all)
    ```shell
    cp [source] [dest]
    ```
  - Move File(cut file)
    [manual](http://man.he.net/?topic=mv&section=all)
    ```shell
    mv [source] [dest]
    ```
  - Zip  
    [manual](http://man.he.net/?topic=zip&section=all)
    ```shell
    zip [output] [source] 
    ```
    Use ```*``` to indicate all files in the directory
  - Unzip
    [manual](http://man.he.net/?topic=unzip&section=all)
    ```shell
    unzip [file]
    ```
<!------------------------------------------------------------------->
