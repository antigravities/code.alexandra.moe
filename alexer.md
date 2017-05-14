# Alexer
A scripting language for world generation.

## Basic language syntax

### Comments
Are denoted with 1 `#`. Comments can only be at the start of a line.

### Indentation
Is not required, but recommended.

### `lines`
When declaring `if`, `while`, or `for` structures, you must define the number of lines that are enclosed within each structure including the initial declaration

### Operators
#### `x = y`
`x` is exactly equal to `y`.
#### `x > y`
`x` is greater than `y`.
#### `x >= y`
`x` is greater than or equal to `y`.
#### `x <= y`
`x` is less than or equal to `y`.

### Variables
Are set with [`assign`](#assign) and can be used within code using the `$` prefix.

## Procedures

### assign
*Arguments: str float*

Assigns a number to a variable. This variable can then be accessed in code by using the prefix `$`.

#### Example
```
assign something 1
print $something
```
```
1
```

### while
*Arguments: float str float (int)*

Executes while the condition `float str float` is true. `str` can be any of those operators defined 

The default for the last argument, `lines`, is 2. See [`lines`](#lines) for more information.

#### Example
```
assign i 0
while $i < 10 3
  print $i
  add i $i 1
```
```
0
1
2
3
4
5
6
7
8
9
```
