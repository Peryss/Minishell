# Minishell
About the Minishell Project

You can find the original Minishell repository here
, developed collaboratively with @her-username
.

Summary

The goal of this project was to recreate a simple version of bash.

This project was part of the 42 Vienna curriculum and focused on implementing core shell functionalities such as command execution, parsing, process management, and signal handling.

My Contributions

I worked on the project together with @her-username
.
My main contributions included:

Designing and implementing the syntax analyzer using a shift-reduce algorithm

Developing the execution module, including pipes, redirections, and process management

Implementing signal handling and creating the global signal structure (t_signals)

Setting up the Docker environment for consistent development

Debugging and testing built-in commands and redirections

Allowed External Functions

readline, rl_clear_history, rl_on_new_line, rl_replace_line, rl_redisplay, add_history,
printf, malloc, free, write, access, open, read, close,
fork, wait, waitpid, wait3, wait4, signal, sigaction, sigemptyset,
sigaddset, kill, exit, getcwd, chdir, stat, lstat, fstat,
unlink, execve, dup, dup2, pipe, opendir, readdir, closedir,
strerror, perror, isatty, ttyname, ttyslot, ioctl,
getenv, tcsetattr, tcgetattr, tgetent, tgetflag, tgetnum,
tgetstr, tgoto, tputs.

Mandatory Part

After running make, your program should be executed as ./minishell and behave like bash.
It should:

Display a prompt

Save command lines to history (accessible with the up and down arrows)

Execute commands with relative and absolute paths

Use only one global variable to store received signals

Handle:

' and " quotes

<, <<, >, and >> redirections

| pipes

$? expansion for the latest exit status

$ expansion for environment variables

Handle signals like bash:

Ctrl-C → display a new prompt on a new line

Ctrl-D → exit the shell

Ctrl-\ → do nothing

Implement the following builtins:

echo with the -n option

cd with relative or absolute path

pwd with no options

export with no options

unset with no options

env with no options or arguments

exit with no options
