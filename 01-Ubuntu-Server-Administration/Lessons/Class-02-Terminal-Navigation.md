# Class 2 — Linux Terminal Navigation

**Status:** Lesson completed  
**Learning path:** Ubuntu Server Administration

## Learning objective

Learn how to move around the Linux filesystem from the terminal and inspect directories and files.

## Core commands

| Command | Purpose | Example |
|---|---|---|
| `pwd` | Print the current working directory | `pwd` |
| `ls` | List directory contents | `ls` |
| `ls -l` | Show a detailed listing | `ls -l` |
| `ls -a` | Include hidden files | `ls -a` |
| `cd` | Change directory | `cd /etc` |
| `cd ..` | Move to the parent directory | `cd ..` |
| `cd ~` | Return to the user's home directory | `cd ~` |
| `cd /` | Move to the filesystem root | `cd /` |
| `clear` | Clear the terminal display | `clear` |
| `man` | Open a command's manual page | `man ls` |

## Absolute and relative paths

- An **absolute path** starts from the filesystem root, such as `/etc/ssh`.
- A **relative path** is interpreted from the current working directory, such as `Documents` or `../Downloads`.

## Suggested practice sequence

Run these commands in the Ubuntu Server terminal and observe how the working directory changes:

```bash
pwd
ls
ls -la
cd /
pwd
ls
cd /etc
pwd
cd ..
pwd
cd ~
pwd
```

## Practical verification

Record the commands you ran, what each output showed, and any navigation exercise you completed. Add screenshots of your own terminal output when available.

## Reflection

Terminal navigation is a foundational Linux administration skill. It helps an administrator locate configuration files, inspect directories, and work efficiently on servers that may not have a graphical desktop.

## Next steps

Continue practising paths and directory navigation, then progress to file and directory management.
