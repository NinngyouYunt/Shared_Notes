# Reference List

Also refer to <CS246>(https://www.student.cs.uwaterloo.ca/~cs246/) course site for more resource

## Linux Shell

### General
- Display command help
  ```s
  man <command>__
  ```
- Clear the the screen
  ```s
  clear
  ```
- Input Redirection
  ```s
  <command> < <file>
  ```
- Output Redirection
  ```s
  <command> > <file>
  ```
- Globbing Pattern (* will match everything)
  ```s
  *.txt
  ```
- Embedded Command
  ```s
  $(<command>)
  ``` 
- Shortcut  
  ```^L ``` for clear screen  
  ```^C``` for terminating program  
  ```^D``` for eol (End of Line) signal  
### Navigation
- Navigate in to folder
  ```s
  cd <path>
  cd ~
  cd ..
  ```
  `~` is used for going to root  
  `..` is for going up the directory tree (to parent folder)
- Display files/directories in current directory  
  <manual>(http://man.he.net/?topic=ls&section=all)
  ```s
  ls <option>
  ```
  Some common options are  
  `-a` for all file (include hidden files)
- Display path
  ```s
  pwd
  ```
- Read file  
  <manual>(http://man.he.net/?topic=cat&section=all)
  ```s
  cat <file>
  ```
- Count  
  <manual>(http://man.he.net/?topic=wc&section=all)
  ```s
  wc <file>
  ```
  Some options are  
  `-c` print the byte count
  `-m` print the character count
  `-l` print the line count
  `-w` print the word count
<!-------------------------------------------------------------------------->
### File/Folder Manipulation
- Create Directory  
  <manual>(http://man.he.net/?topic=mkdir&section=all)
  ```s
  mkdir <folder>
  ```
- Remove Directory (if it's empty)
  <manual>(http://man.he.net/?topic=rmdir&section=all)
  ```s
  rmdir
  ```
- Remove Directory (and all children)
  ```s
  rm -r <folder>
  ```
- Remove File  
  <manual>(http://man.he.net/?topic=rm&section=all)
  ```s
  rm <file>
  ```
- Copy File  
  <manual>(http://man.he.net/?topic=cp&section=all)
  ```s
  cp <source> <dest>
  ```
- Move File(also used to rename)
  <manual>(http://man.he.net/?topic=mv&section=all)
  ```s
  mv <source> <dest>
  ```
- Zip  
  <manual>(http://man.he.net/?topic=zip&section=all)
  ```s
  zip <output> <source> 
  ```
  Use ```*``` to indicate all files in the directory
- Unzip
  <manual>(http://man.he.net/?topic=unzip&section=all)
  ```s
  unzip <file>
  ```
<!------------------------------------------------------------------->
### Scripting
- General
  - Comments
    ```s
    # This ia comment
    ```
  - Quote
    ```' '``` Single quotes escape everything inside and the bash treats as __string literal__
    ```" "``` Double quotes escape __globbing pattern__ 
  - Script Starting (used to indicate type of program, given example is for bash)
    ```s
    #!/bin/bash
    ``` 
- Variables
  - Declaration
    ```s
    a=123
    # No space before and after '='
    ```
  - Access
    ```s
    ${longName} # Recommanded
    $var # If followed by other variable/used in speical case, it will be different
    echo $var1 # This would print variable var1 instead of var followed by a "1"
    ```
  - Drop Suffix
    ```s
    ${<var>%<suffix>} # will attempt to drop suffix from the varaible if it is there
    ```
- Flow Control
  - If Statement  
    __There must be ``` ``` after ```[``` and before ```]```__
    ```s
    if [ <cond> ]; then
      ...
    elif [ <cond> ]; then
      ...
    fi
    ```
  - Loop
    - For Loop  
      __The ```<string>``` can be a literal string(which will be matched to globbing pattern is not enclosed) or variables__
      ```s
      for <var> in <string> do
        ...
      done
      ```
    - While Loop  
      __Same rule as ___For Loop___ for the ```[ ]```__
      ```
      while [ <cond> ] do
        ...
      done
      ```
