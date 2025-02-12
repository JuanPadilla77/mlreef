# Edit files through the command line

When [working with Git from the command line](1-start_using_git.md), you will need to
use more than just the Git commands. There are several basic commands that you should
learn, in order to make full use of the command line.

## Start working on your project

To work on a Git project locally (from your own computer), with the command line,
first you will need to [clone (copy) it](start-using-git.md#clone-a-repository) to
your computer.

## Working with files on the command line

This section has examples of some basic shell commands that you might find useful.
For more information, search the web for _bash commands_.

Alternatively, you can edit files using your choice of editor (IDE), or the MLReef user
interface (not locally).

### Common commands

The list below is not exhaustive, but contains many of the most commonly used commands.

| Command                        | Description                                 |
|--------------------------------|---------------------------------------------|
| `cd NAME-OF-DIRECTORY`         | Go into a directory to work in it           |
| `cd ..`                        | Go back one directory                       |
| `ls`                           | List what’s in the current directory        |
| `ls a*`                        | List what’s in the current directory that starts with `a` |
| `ls *.md`                      | List what’s in the current directory that ends with `.md` |
| `mkdir NAME-OF-YOUR-DIRECTORY` | Create a new directory                      |
| `cat README.md`                | Display the contents of a [text file you created previously](#create-a-text-file-in-the-current-directory) |
| `pwd`                          | Show the current directory                  |
| `clear`                        | Clear the shell window                      |

### Create a text file in the current directory

To create a text file from the command line, for example `README.md`, follow these
steps:

```shell
touch README.md
nano README.md
#### ADD YOUR INFORMATION
#### Press: control + X
#### Type: Y
#### Press: enter
```

### Remove a file or directory

It is easy to delete (remove) a file or directory, but be careful:

DANGER: **Danger:**
This will **permanently** delete a file.

```shell
rm NAME-OF-FILE
```

DANGER: **Danger:**
This will **permanently** delete a directory and **all** of its contents.

```shell
rm -r NAME-OF-DIRECTORY
```

### View and Execute commands from history

You can view the history of all the commands you executed from the command line,
and then execute any of them again, if needed.

First, list the commands you executed previously:

```shell
history
```

Then, choose a command from the list and check the number next to the command (`123`,
for example) . Execute the same full command with:

```shell
!123
```

### Carry out commands for which the account you are using lacks authority

Not all commands can be executed from a basic user account on a computer, you may
need administrator's rights to execute commands that affect the system, or try to access
protected data, for example. You can use `sudo` to execute these commands, but you
will likely be asked for an administrator password.

```shell
sudo RESTRICTED-COMMAND
```

CAUTION: **Caution:**
Be careful of the commands you run with `sudo`. Certain commands may cause
damage to your data or system.

## Sample Git taskflow

If you are completely new to Git, looking through some [sample taskflows](https://rogerdudler.github.io/git-guide/)
will help you understand the best practices for using these commands as you work.
