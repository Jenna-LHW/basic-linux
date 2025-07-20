# File and Directory Operations

## `ls` command 
`ls` command is used to **list the contents of a directory**. 

Basic Syntax:
```
ls [options] [directories]
```
Some common Usage:
| Command              | Description                                                    |
| -------------------- | -------------------------------------------------------------- |
| `ls`                 | Lists files and directories in the current dir                 |
| `ls /home/user`      | Lists contents of the `/home/user` directory                   |
| `ls -l`              | Long listing format (shows permissions, size, etc.)            |
| `ls -a`              | Shows **all** files, including hidden ones (`.` prefix)        |
| `ls -la` or `ls -al` | Long format including hidden files                             |
| `ls -lh`             | Long listing with **human-readable** file sizes (e.g., KB, MB) |
| `ls -lt`             | Sorts files by **modification time**, newest first             |
| `ls -R`              | Lists **recursively**, showing subdirectories too              |
| `ls -d */`           | Lists **only directories** in the current folder               |

## `cd` command
`cd` command is used to change the current working directory.

Basic Syntax:
```
cd [directory]
```
Some Common Usage:
| Command           | Description                                   |
| ----------------- | --------------------------------------------- |
| `cd`              | Go to the **home** directory                  |
| `cd ~`            | Also goes to the home directory               |
| `cd /`            | Go to the **root** directory (`/`)            |
| `cd ..`           | Go **up one level** (to the parent directory) |
| `cd ../..`        | Go up **two levels**                          |
| `cd foldername`   | Enter a subdirectory named `foldername`       |
| `cd /path/to/dir` | Go to a specific path (absolute path)         |
| `cd -`            | Switch to the **previous** directory          |

# `pwd` command
`pwd` command stands for "**print working directory**". It shows the path of the current directory you are in.

Basic Syntax:
```
pwd [options]
```

Example:
```
$ pwd
/home/jenna
```

# `mkdir` command
`mkdir` command stands for "**make directories**". It used to create new directories (folders).

Basic Syntax:
```
mkdir [options] <directory_name>
```

Some Common Usage:
| Command               | Description                                     |
| --------------------- | ----------------------------------------------- |
| `mkdir myfolder`      | Creates a folder named `myfolder`               |
| `mkdir Projects/Code` | Creates `Code` **inside** the `Projects` folder |
| `mkdir -p a/b/c`      | Creates nested directories (`a`, `b`, and `c`)  |

> **Note**: Without `-p`, `mkdir a/b/c` will give an error if a or b don't exist.

# `rmdir` command
`rmdir` command is used to **remove empty directories**.

Basic Syntax:
```
rmdir [options] <directory_name>
```

Some common Usage:
| Command          | Description                                          |
| ---------------- | ---------------------------------------------------- |
| `rmdir myfolder` | Removes the `myfolder` directory **if empty**        |
| `rmdir a/b/c`    | Removes `c` if it's empty (not `a` or `b`)           |
| `rmdir -p a/b/c` | Removes `c`, then `b`, then `a` **if all are empty** |


**Important**
- `rmdir` only works on empty folders.
- If the folder is not empty, you'll get an error.

# `rm` command 
`rm` command is used to remove (delete) files and directories.

Basic command:
```
rm [options] <files/directories>
```
Some Common Usage:
| Command          | Description                                        |
| ---------------- | -------------------------------------------------- |
| `rm file.txt`    | Deletes a file named `file.txt`                    |
| `rm *.txt`       | Deletes **all `.txt` files** in the current folder |
| `rm -i file.txt` | Prompts **confirmation** before deleting           |
| `rm -r folder/`  | Deletes a **folder and its contents** recursively  |
| `rm -rf folder/` | Force deletes a folder **without asking**          |

> **Dangerous command**
> ```
> rm -rf /
> ```
> This will try to delete **everthing on your system.**  
> **Never run this**

# `cp` command
`cp` command is used to **copy files and directories**.

Basic Syntax:
```
cp [options] <source> <destination>
```

Somme commnon Usage:
| Command                    | Description                                           |
| -------------------------- | ----------------------------------------------------- |
| `cp file.txt backup.txt`   | Copies `file.txt` to a new file called `backup.txt`   |
| `cp file.txt /home/jenna/` | Copies file to another directory                      |
| `cp -i file.txt /folder/`  | Prompts before overwriting an existing file           |
| `cp -r folder1 folder2`    | Recursively copies directory `folder1` into `folder2` |
| `cp *.txt /backup/`        | Copies all `.txt` files to `/backup/` directory       |

# `mv` command
`mv` command is used to move files and directories

Basic Syntax:
```
mv [options] <source> <destination>
```

Some Common Usage:
| Command                    | Description                                        |
| -------------------------- | -------------------------------------------------- |
| `mv file.txt /home/jenna/` | Moves `file.txt` to the `/home/jenna/` directory   |
| `mv file.txt newname.txt`  | **Renames** `file.txt` to `newname.txt`            |
| `mv oldfolder/ /backup/`   | Moves `oldfolder` (and its contents) to `/backup/` |
| `mv *.txt /archive/`       | Moves all `.txt` files to `/archive/`              |

