# Shell Scripts

## What is a shell script?

A shell script is a text file that contains a series of commands that can be executed by the shell. The shell is a program that interprets and executes commands. The most common shell on Linux is bash.

## How to write a shell script

To write a shell script, you can use any text editor. The following is an example of a simple shell script:

``` shell
#!/bin/bash

echo "Hello, world!"
echo "The current date and time is $(date)"
```

This script will print the message "Hello, world!" to the console.

## How to run a shell script

To run a shell script, you can use the following command:

``` shell
bash <script_name>
```

For example, to run the script above, you would use the following command:

``` shell
bash hello_world.sh
```

## Variables

Variables are used to store data in shell scripts. To declare a variable, you use the following syntax:

``` shell
variable_name=value
```

For example, the following code declares a variable named name and assigns it the value "John Doe":

``` shell
name="John Doe"
```

You can then access the value of the variable by using its name. For example, the following code will print the value of the `name` variable:

``` shell
echo $name
```

## Conditional statements

Conditional statements are used to control the flow of execution in shell scripts. The most common conditional statements are `if`, `else`, and `elif`:

* The `if` statement is used to execute a block of code if a condition is met.
* The `else` statement is used to execute a block of code if the condition in the `if` statement is not met.
* The `elif` statement is used to execute a block of code if a condition is met, but the condition in the `if` statement is not met.
  
For example, the following code will print the message "Hello, world!" if the variable `name` is not empty:

``` shell
if [ -n "$name" ]; then
  echo "Hello, $name!"
fi
```

## Loops

Loops are used to execute a block of code repeatedly. The most common loops are `for` and `while`:

* The `for` loop is used to iterate over a list of items.
* The `while` loop is used to execute a block of code as long as a condition is met.

For example, the following code will print the names of all the files in the current directory:

``` shell
for file in *; do
  echo $file
done
```

## Functions

Functions are used to group together a set of commands that can be executed repeatedly. To define a function, you use the following syntax:

``` shell
function_name() {
  <block of code>
}
```

For example, the following code defines a function named `greet` that prints the message "Hello, world!" to the console:

``` shell
function greet() {
  echo "Hello, world!"
}
```

You can then call the function by using its name. For example, the following code will call the `greet` function:

``` shell
greet
```

## Output redirection

Output redirection is used to redirect the output of a command to a file. To redirect output to a file, you use the following syntax:

``` shell
command > output_file
```

For example, the following code will redirect the output of the `ls` command to the file `list.txt`:

``` shell
ls > list.txt
```

## Input redirection

Input redirection is used to redirect input to a command from a file. To redirect input from a file, you use the following syntax:

``` shell
command < input_file
```

For example, the following code will read the contents of the file `list.txt` and print them to the console:

``` shell
cat list.txt
```

## Error handling

Error handling is used to deal with errors that occur in shell scripts. The most common way to handle errors is to use the `try` and `catch` statements:

* The `try` statement is used to execute a block of code.
* The `catch` statement is used to handle errors that occur in the try block.

For example, the following code will try to create a directory named `new_dir`. If the directory already exists.

## Examples of Bash in Bioinformatics

* [Introduction To Bash: Using the Terminal For Bioinformatics](https://uofabioinformaticshub.github.io/BASH-Intro/). University of Adelaide.
* [Process fasta script](https://github.com/pavlohrab/process_fasta). Pavlo Hrab.
* [Samtools: faidx](http://www.htslib.org/doc/faidx.html)

### References

* [The Command Line Interface Shell](https://github.com/clizarraga-UAD7/Workshops/wiki/The-Command-Line-Interface-Shell)
* [UNIX Shell Command Line Programming](https://github.com/clizarraga-UAD7/Workshops/wiki/UNIX-Shell---Command-Line-Programming)
* [Loops](https://swcarpentry.github.io/shell-novice/05-loop.html)
* [explainshell.com](https://explainshell.com/)

***

Created: 05/16/2023: Updated: 05/17/2023

Carlos Lizárraga
