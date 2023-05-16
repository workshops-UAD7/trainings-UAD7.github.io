# Pipes and Filters in Unix


## Common Unix command used as pipes and filters

The most common pipes and filters used in Unix are:

| Command | Description |
| :--: | :-- |
| [`grep`](https://man7.org/linux/man-pages/man1/grep.1.html) | Text search utility that can be used to find specific patterns of text in a file or stream |
| [`sort`](https://man7.org/linux/man-pages/man1/sort.1.html)  | Utility that can be used to sort the lines of a file | 
| [`uniq`](https://man7.org/linux/man-pages/man1/uniq.1.html)  |  Utility that can be used to remove duplicate lines from a file |
| [`head`](https://man7.org/linux/man-pages/man1/head.1.html) | Utility that can be used to print the first few lines of a file |
| [`tail`](https://man7.org/linux/man-pages/man1/tail.1.html) | Utility that can be used to print the last few lines of a file |
| [`wc`]() | - Utility that can be used to count the number of lines, words, and characters in a file |

These utilities can be combined to create powerful pipelines that can be used to perform a variety of tasks.

## Examples

| Command | Description |
| :--  | :-- |
| `grep -n hello file.txt` | Find all of the occurrences of the word "hello" in a file and print the line numbers |
| `sort file.txt | head -10` | Sort the lines of a file and then print the first 10 lines |
| `sort file.txt | uniq -d` |  Find all of the duplicate lines in a file and print them |

## The use of pipes '|','>', 'tee',  and '>> ' in Unix

**Pipes ('|')**

A pipe is a way of connecting the output of one command to the input of another command. This allows you to chain together commands and perform complex operations on data.
```
ls -l | sort 
```
The `ls` command will list the files in the current directory, and the `sort` command will sort the list by name. The output of the `ls` command will be piped to the input of the `sort` command, so that sort can operate on the list of files.

**Redirection ('>')**

Redirection is a way of changing the destination of a command's output. This can be used to save the output of a command to a file, or to display the output on the screen.
```
ls -l > files.txt
```
The ls command will list the files in the current directory, and the output will be redirected to the file files.txt.


**tee**

The tee command is a utility that can be used to copy the output of a command to multiple destinations. This can be useful for logging output to a file, or for sending output to both the screen and a file.
```
ls -l | tee files.txt
```
The `ls` command will list the files in the current directory, and the output will be sent to both the screen and the file `files.txt`.

**Append redirection ('>>')**

Append redirection is a way of adding the output of a command to the end of a file. This can be used to append the output of a command to an existing file, or to create a new file with the output of a command.
```
ls -l >> files.txt
```
The `ls` command will list the files in the current directory, and the output will be appended to the file `files.txt`.

## Examples

Some examples of how pipes, redirection, and `tee` can be used together:

| Command | Description |
| :-- | :-- |
| `ls -l >> files.txt` | list all of the files in the current directory and append the list to the file `files.txt` |
| `ls -l | grep hello` | find all of the files in the current directory that contain the word "hello"  | 
| `sort file.txt | head -10` | sort the lines of a file and then print the first 10 lines | 
| `sort file.txt | uniq -d` | find all of the duplicate lines in a file and print them | 
| `command | tee log.txt` | log the output of a command to a file | 
| `command | tee -a screen.txt` | send the output of a command to both the screen and a file |

### References

* [The Command Line Interface Shell](https://github.com/clizarraga-UAD7/Workshops/wiki/The-Command-Line-Interface-Shell)
* [Pipes and Filters](https://swcarpentry.github.io/shell-novice/04-pipefilter.html)
* [explainshell.com](https://explainshell.com/)

   
***

Created: 05/13/2023: Updated: 05/15/2023,<br>
Carlos Lizárraga

