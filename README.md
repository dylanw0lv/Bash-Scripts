# Bash-Scripts


## Vanilla JavaScript Boilerplate Setup for Command Line on Ubuntu

To execute the script from the command line, you can add an alias. 
In Linux, an alias is a custom shortcut that references a command.


### Temporary Alias

For example:

Instead of typing 'clear' to clear the console,
you can add an alias for the clear command.

```
alias c='clear'
```

This command would add 'c' as a command that references clear.


There is only one problem:

When aliases are created using this command, they are temporary aliases.
They will not work after the current instance of the terminal is closed.


### Permanent Alias

To add a permanent alias, you need to create a file a new file in the root directory.

Run this command in the root directory:

```
touch .bash_aliases
```
Next, you can open the file you created in your text editor of choice.

To open in VS Code run the command:

```
code .bash_aliases
```

Open in nano:

```
nano .bash_aliases
```


To run a bash script, this command can be executed in the console:

```
source [filename]
```

Instead of typing out this long command, you can create an alias. Enter the alias command into the file .bash_aliases.

For example:

```
alias cproj='source ~/Desktop/Projects/Bash-Scripts/vanillaJS_boilerplate.sh'
```

After this alias is added to my .bash_aliases file, I can type 'cproj' in the console and it runs my script.