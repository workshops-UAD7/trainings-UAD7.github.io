# Working with files and directories

In this section we will focus on files and directories.

In Unix, files and directories are similar

A [computer file](https://en.wikipedia.org/wiki/Computer_file) is a named collection of data that is stored on a computer's hard drive or other storage device. Files can contain text, images, audio, video, and other types of data. Files are typically opened and closed using a file manager or other software application.

A [directory](https://en.wikipedia.org/wiki/Directory_(computing)) is a named collection of files and other directories. Directories are used to organize files and make them easier to find. Directories are typically opened and closed using a file manager or other software application.

## Similarities and differences between files and Directories

### Similarities

* Both files and directories are stored on the same physical disk.
* Both files and directories have names.
* Both files and directories can be owned by users and groups.
* Both files and directories can have permissions set on them.
* Both files and directories can be accessed using the same commands.

### Differences

* A file is a collection of data, while a directory is a collection of files.
* A file cannot contain other files, while a directory can contain other files and directories.
* A file can be accessed directly by its name, while a directory can only be accessed by navigating to it through the file system hierarchy.

## List of commands for working with Files and Directories

The following table shows some of the main Unix commands for working with files and directories:

| Command | Description |
| :--: | :-- |
| [`ls`](https://man7.org/linux/man-pages/man1/ls.1.html) |  List the contents of a directory |
| [`cd`](https://man7.org/linux/man-pages/man1/cd.1p.html) |  Change the current directory |
| [`mkdir`](https://man7.org/linux/man-pages/man1/mkdir.1.html) |  Create a new directory |
| [`rmdir`](https://man7.org/linux/man-pages/man1/rmdir.1.html) | Remove an empty directory |
| [`touch`](https://man7.org/linux/man-pages/man1/touch.1.html) | Create a new empty file |
| [`cat`](https://man7.org/linux/man-pages/man1/cat.1.html) | Display the contents of a file |
| [`cp`](https://man7.org/linux/man-pages/man1/cp.1.html) | Copy a file |
| [`mv`](https://man7.org/linux/man-pages/man1/mv.1.html) | Move a file |
| [`rm`](https://man7.org/linux/man-pages/man1/rm.1.html) | Remove a file :warning: |
| [`more`](https://man7.org/linux/man-pages/man1/more.1.html) | Display the contents of a file one screen at a time |
| [`less`](https://man7.org/linux/man-pages/man1/less.1.html) |  Display the contents of a file one screen at a time and allow scrolling |
| [`head`](https://man7.org/linux/man-pages/man1/head.1.html) | Output the first part of file |
| [`tail`](https://man7.org/linux/man-pages/man1/tail.1.html) | Output the last part of file |
| [`grep`](https://man7.org/linux/man-pages/man1/grep.1.html) | Search for a pattern in a file |
| [`sort`](https://man7.org/linux/man-pages/man1/sort.1.html) | Sort the lines in a file |
| [`uniq`](https://man7.org/linux/man-pages/man1/uniq.1.html) |  Remove duplicate lines from a file |
| [`find`](https://man7.org/linux/man-pages/man1/find.1.html) | Find files that match a certain criteria |
| [`chmod`](https://man7.org/linux/man-pages/man1/chmod.1.html) | Change the permissions on a file |
| [`chown`](https://man7.org/linux/man-pages/man1/chown.1.html) | Change the ownership of a file |
| [`ln`](https://man7.org/linux/man-pages/man1/ln.1.html) | Create a link to a file |
| [`tar`](https://man7.org/linux/man-pages/man1/tar.1.html) | Create a compressed archive of a file or directory |
| [`gzip`](https://ss64.com/bash/gzip.html) | Compress or decompress a file |
| [`bzip2`](https://ss64.com/bash/bzip2.html) | Compress or decompress a file |

### References

* [The Command Line Interface Shell](https://github.com/clizarraga-UAD7/Workshops/wiki/The-Command-Line-Interface-Shell)
* [Working with Files and Directories](https://swcarpentry.github.io/shell-novice/03-create.html)
* [explainshell.com](https://explainshell.com/)
  
***

Created: 05/13/2023: Updated: 05/15/2023

Carlos Lizárraga
