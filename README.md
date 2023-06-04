# Ark Programming Language Documentation

## Introduction

Ark is a programming language designed to be simple and efficient. This document provides an overview of the Ark programming language and its syntax. It covers the basic concepts and features of the language, including functions, loops, and printing.

## Syntax

### Function Definitions

To define a function in Ark, use the `FUN` keyword followed by the function name and parameter list. The function body is enclosed in a block using indentation.

```ark
FUN oopify(prefix) -> prefix + "oop"
```

### Function Calls

To call a function in Ark, simply use the function name followed by parentheses and arguments.

```ark
result = oopify("Ark")
```

### Variable Declarations

To declare a variable in Ark, use the `VAR` keyword followed by the variable name and an optional initial value.

```ark
VAR result = ""
VAR len = LEN(elements)
```

### Control Flow

Ark supports loops and conditional statements.

#### For Loop

To iterate over a range of values in Ark, use the `FOR` loop. It requires a loop variable, a start value, an end value, and an optional step value.

```ark
FOR i = 0 TO len THEN
    result = result + elements/i
    IF i != len - 1 THEN result = result + separator
END
```

#### Conditional Statement

Ark uses the `IF` keyword for conditional statements. It requires a condition and a block of code to execute if the condition is true.

```ark
IF i != len - 1 THEN
    result = result + separator
END
```

### Return Statement

To return a value from a function in Ark, use the `RETURN` keyword followed by the value to be returned.

```ark
RETURN result
```

### Printing

To display output in Ark, use the `PRINT` statement followed by the value or expression to be printed.

```ark
PRINT("Greetings universe!")
```

### Example Usage

Here's an example usage of the functions defined in Ark:

```ark
FOR i = 0 TO 5 THEN
    PRINT(join(map(["l", "sp"], oopify), ", "))
END
```

This code will iterate five times and print the joined and oopified elements from the given list.

## Conclusion

This concludes the documentation for the Ark programming language. It provides an overview of the syntax and features of the language. You can now start writing programs in Ark using the provided functions and concepts. Happy coding!
