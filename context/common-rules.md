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

Always follow the above rules.
