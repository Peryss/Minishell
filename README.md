# About the Minishell Project

You can find the original Minishell repository [here](https://github.com/cseriildi/minishell), developed collaboratively with [@cseriildi](https://github.com/cseriildi).

---

## Summary

The goal of this project was to recreate a simple version of **bash**.

This project was part of the **42 Vienna curriculum** and focused on implementing core shell functionalities such as command execution, parsing, process management, and signal handling.

---

## My Contributions

I worked on the project together with [@cseriildi](https://github.com/cseriildi).  
My main contributions included:

- Designing and implementing the **syntax analyzer** using a **shift-reduce algorithm**  
- Developing the **execution module**, including pipes, redirections, and process management  
- Implementing **signal handling** and creating the global signal structure (`t_signals`)  
- Debugging and testing built-in commands and redirections  

---

## Functionalities

After running `make`, your program should be executed as `./minishell` and behave like **bash**.  
It should:

- Display a prompt  
- Save command lines to history (accessible with the up and down arrows)  
- Execute commands with relative and absolute paths  
- Use only one global variable to store received signals  
- Handle:
  - `'` and `"` quotes  
  - `<`, `<<`, `>`, and `>>` redirections  
  - `|` pipes  
  - `$?` expansion for the latest exit status  
  - `$` expansion for environment variables  
- Handle signals like bash:
  - **Ctrl-C** → display a new prompt on a new line  
  - **Ctrl-D** → exit the shell  
  - **Ctrl-\\** → do nothing  
- Implement the following builtins:
  - `echo` with the `-n` option  
  - `cd` with relative or absolute path  
  - `pwd` with no options  
  - `export` with no options  
  - `unset` with no options  
  - `env` with no options or arguments  
  - `exit` with no options  
