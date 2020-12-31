# ffufez

> ffufez - A simple script to run ffuf for lazy people.

This is a script I wrote to automate the mundane chore of typing in the lengthy ffuf command especially if you have all the arguments set.

---
## Features

This script allows you to input the following:
- Input URL/FUZZ
- Select from the options of wordlists 
   - Currently uses raft and dirbuster wordlists or you can specify a custom one
- Input your desired extensions or use the (-all) to-do common extensions
- Recursive on or off
- Saves the scan results in your current PWD


## Requirements

- bash
- ffuf (get it [here](https://github.com/ffuf/ffuf))
- seclists (get it [here](https://github.com/danielmiessler/SecLists))

## Installation

- git clone 'https://github.com/dalemazza/ffufez.git'
- chmod +x ffufez

If you want to run this script globally you can add it your $PATH

## Usage example

```
./ffufez
~~ffufez~~
Input URL (URL/FUZZ): 10.10.10.10/FUZZ
~~Wordlists~~
Select Worldlist 1-2: 
1. raft-small-directories
2. directory-list-2.3-medium
Custom - Please type full file path
: 1
~~Extensions~~
Input manually in this format .txt,.html etc
Automatic -all to use common extensions
: -all
~~Recursive~~
Yes/No: yes
Scan will be saved here /home/kali
        /'___\  /'___\           /'___\       
       /\ \__/ /\ \__/  __  __  /\ \__/       
       \ \ ,__\\ \ ,__\/\ \/\ \ \ \ ,__\      
        \ \ \_/ \ \ \_/\ \ \_\ \ \ \ \_/      
         \ \_\   \ \_\  \ \____/  \ \_\       
          \/_/    \/_/   \/___/    \/_/       
```

## Issues

Currently this script has no error handling so please ensure you use the options provided or you will get errors!
