# Quality of Life - Bash
Some configuration you can do to Linux bash  
  

## How to change PuTTY color scheme
1. Get a ```*.reg ``` file for PuTTY color scheme  
   - Like [this](https://github.com/AlexAkulov/putty-color-themes)
2. Update the section (change ```<session>``` to your saved session)
   - ```[HKEY_CURRENT_USER\Software\SimonTatham\PuTTY\Sessions\<session>]```
3. Import the file into your registry

## Change prompt ($PS1)
- Direct Change
  - use command ```$PS1="your own prompt"```
- Save change
  - Add ```PS1="your stuff"``` into ```~/.bash_profile```
- Some avaiable stuff
  - | Character | What It Prints    |
    |-----------|-------------------|
    | ```\h```  | hostname          |
    | ```\u```  | user              |
    | ```\W```  | current directory |
- Change Color (try different number other than 33)
  - ```\e[1;33m<what you want to put>\e[0m```

## Add folder to PATH
1. Add following to your ```~/.bash_profile```
   - ```PATH=$PATH:<path to your folder>```

## Vim 
- Tmux allow you to split window
  - run ```tmux```
  - To split use ```C-b %``` (Ctrl-b + %)
  - To navigate use ```C-b arrow```
  - To close current panel ```C-b x```
  - Help use ```C-b ?```
  - [CheatSheet](https://tmuxcheatsheet.com/)
- Youcompleteme allow auto complete
- .vimrc
  - Add ```set number``` to allow display of line number
  - Add ```set expandtab``` to make Tab key into entering spaces
  - Add ```set tabstop=2``` to make Tab key entering 2 spaces