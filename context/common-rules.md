# Important rules when writing Risor code
- Use two spaces to indent code
- No `var` keyword for variables (use `:=`)
- No `??` operator for null coalescing (use `coalesce()` function)
- Module imports don't use quotes. Use `import math` and not not `import "math"`
- Use single quotes for string interpolation: `'Hello, {name}'`
- If-else and switch are expressions that return values
- String interpolation with single quotes only supports simple variable substitution (`'{variable}'`). It does not support formatting specifications inside the curly braces like Python's f-strings. To format values, use the `fmt.sprintf()` function separately and concatenate the results
- ^ is not a valid power operator in Risor. Use math.pow() function instead
- Use os.stdin.input() to read input from the user
- Risor doesn't have while to create loops. Always use for and range.
- Risor doesn't have __main__ or __file__ globals
- Risor doesn't support variadic arguments when calling or defining functions
- Lists in Risor behave very similarly to lists in Python. Methods and indexing
on lists are the primary way to interact with these objects. A list can store
objects of any types, including a mix of types in one list.

```go
>>> l := ["a", 1, 2]
["a", 1, 2]
>>> l.append("tail")
["a", 1, 2, "tail"]
```
- Reserved keywords:
  - func
  - import
  - return
  - if
  - for
  - range
  - spawn
  - from

Always follow the above rules.
