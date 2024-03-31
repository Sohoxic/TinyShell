
# TinyShell: A Minimalist Shell Implementation in C

TinyShell is a simple, minimalist shell implementation written in C, designed for educational purposes. It demonstrates the core concepts of how a shell works, including reading input, parsing commands, and executing system commands or built-in functions.

## Features

- Basic command parsing and execution.
- Built-in commands: `cd`, `help`, and `exit`.
- Execution of system commands via `execvp`.
- Simple loop for command input and execution.

## Getting Started

### Prerequisites

To compile and run TinyShell, you need:
- A C compiler (e.g., `gcc`, `clang`).
- Standard development tools (`make`, etc.) if you wish to use a Makefile.

### Compilation

To compile TinyShell, navigate to the source code directory and run:

```bash
gcc -o tinysh main.c
```

### Running TinyShell

After compilation, you can start TinyShell by running:

```bash
./tinysh
```

You will be greeted with a simple prompt (`> `) where you can type your commands.

## Built-in Commands

- `cd [directory]` - Change the current working directory.
- `help` - Display information about built-in commands.
- `exit` - Exit TinyShell.

## Extending TinyShell

To add new built-in commands:
1. Define a new function for the command in the source code.
2. Add the command name and function to the `builtin_str` and `builtin_func` arrays, respectively.
3. Ensure your command function returns `1` to continue execution, or `0` to signal TinyShell to exit.

## License

TinyShell is open-source software distributed under the MIT license. Feel free to modify, distribute, and use it as you see fit.

## Acknowledgments

- This project is inspired by Stephen Brennan's tutorial on writing a shell in C.
- Special thanks to everyone who contributed to testing and providing feedback for TinyShell.

Enjoy experimenting with TinyShell!
