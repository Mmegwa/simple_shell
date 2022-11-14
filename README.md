#!/bin/bash
ALX Simple Shell Project

Displays a prompt "#cisfun$ " and waits for user input.
Runs all commands of type "executable program" (ls and /bin/ls).
Runs the following build_in commands: exit, env, setenv and unsetenv.
Handles commands with arguments.
Handles the PATH global variable.
Handles The EOF (End Of File) condition.
Handles the Ctrl + C signal -> It doesn't exit the shell

Files
1	AUTHORS -> List of contributors to this repository
2	man_1_simple_shell -> Manual page for the simple_shell
3	shell.h -> Header file
4	shell.c -> main function
		sig_handler -> handles the Ctrl + C signal
		_EOF -> handles the End Of File condition
5	string.c
		_putchar -> prints a character
		_puts -> prints a string
		_strlen -> gives the length of a string
		_strdup -> copies a string in a newly allocated memory
		concat_all -> concatenates 3 strings in a newly allocated memory6	line_exec.c
		splitstring -> splits a string into an array of words
		execute -> executes a command using execve
		realloc -> reallocates a memory block
		freearv -> frees a 2 dimensional array
7	linkpath.c
		_getenv -> returns the value of a global variable
		add_node_end -> adds a node in a singly linked list
		linkpath -> creates a singly linked list for PATH directories
		_which -> finds the pathname of a command
		free_list -> frees the linked list of PATH value
8	checkbuild.c
		checkbuild -> checks if a command is a build-in command
9	buildin.c
		exitt -> handles the exit buildin command
		_atoi -> converts a string into an integer
		env -> prints the current environment
		_setenv -> Initialize a new global variable, or modify an existing one
		_unsetenv -> remove a global variable
