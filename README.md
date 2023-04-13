# x! Programming Language

## Introduction
x! (pronounced "x-bang") is a simple, interpreted programming language with a minimalistic syntax. It's designed to be easy to learn and use, with just 11 commands to work with.

## How It Works
When you run a program in x!, the interpreter initializes an empty array. You write one or more character commands to read from and write to this array. Here's a breakdown of how each command works:

- `/` - Moves the selector position up
- `\` - Moves the selector position down
- `.` - Prints the array
- `%` - Prints the current position value
- `|` - Prints a new line
- `#` - Clears the array but position is saved
- `?` - Prints current position
- `$pos;` - Sets the current position value
- `=text;` - Sets the array value at the current position
- `:code;` - Sets the array value but evaluates JS
- `[text]` - Code comments

## Commands

### `/`
Moves the selector position up. If the selector is at the top of the array, it loops back around to the bottom.

### `\`
Moves the selector position down. If the selector is at the bottom of the array, it loops back around to the top.

### `.`
Prints the entire array as a space-separated list.

### `%`
Prints the value at the current selector position.

### `|`
Prints a new line.

### `#`
Clears the entire array, but the selector position is saved.

### `?`
Prints the current selector position.

### `$pos;`
Sets the selector position to the provided position value. For example, `$5;` would set the selector position to 5.

### `=text;`
Sets the value of the current selector position to the provided text. For example, `=hello;` would set the value of the current selector position to "hello".

### `:code;`
Sets the value of the current selector position by evaluating the provided JavaScript code. For example, `:10*2+1;` would set the value of the current selector position to 21.

### `[text]`
Comments in x! start with `[` and end with `]`. Anything inside the comment is ignored by the interpreter.

