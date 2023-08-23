# Simple Shell Project

This is a simple UNIX command line interpreter project for the ALX SE curriculum. The purpose of this project is to create a basic shell that can interpret and execute user commands. The shell supports various functionalities and features outlined in the project requirements.

## Requirements

### General

- Allowed editors: vi, vim, emacs
- All files are compiled on Ubuntu 20.04 LTS using `gcc`, with the options `-Wall -Werror -Wextra -pedantic -std=gnu89`
- All source code files must end with a new line
- A `README.md` file at the root of the project folder is mandatory
- Code should follow the Betty style guidelines, which will be checked using `betty-style.pl` and `betty-doc.pl`
- Shell should not have any memory leaks
- Each source file should contain no more than 5 functions
- All header files should use include guards
- Use system calls only when necessary
- An `AUTHORS` file should be present at the root of the repository, listing all contributors to the project

### Output

The shell should have the same output and error messages as `/bin/sh` for various commands and scenarios.

### List of Allowed Functions and System Calls

- access
- chdir
- close
- closedir
- execve
- exit
- _exit
- fflush
- fork
- free
- getcwd
- getline
- getpid
- isatty
- kill
- malloc
- open
- opendir
- perror
- read
- readdir
- signal
- stat (__xstat)
- lstat (__lxstat)
- fstat (__fxstat)
- strtok
- wait
- waitpid
- wait3
- wait4
- write

## Compilation

The shell will be compiled using the following command:

```bash
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
```

## Testing

The shell should work both in interactive mode and non-interactive mode.

### Interactive Mode

```bash
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($) exit
$
```

### Non-Interactive Mode

```bash
$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
```

## Project Structure

The project is divided into tasks, each building on the previous one. The tasks involve implementing various features and functionalities of a basic shell, such as handling commands, arguments, built-in commands, logical operators, environment variables, and more.

## Authors

- [Wisdom E. Sena](https://github.com/wisdomsena36)
- [Mabel Ablah Zigah](https://github.com/mabrite)
