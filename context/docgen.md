## Documenting Risor function, classes and methods

```go
// Description of the function
// This can span multiple lines
//
// Parameters:
// - param1: Description of first parameter
// - param2: Description of second parameter
//
// Returns: Description of what is returned
```

### Class or Function Annotations

The tool looks for special annotation comments:

- `@object.class` - Marks a class declaration
- `@object.method` - Marks a class method
- `@global.function` - Marks a global function

## Example

Input Risor file:

```go
// Prints a string
//
// Parameters:
// - msg: string to print
//
// @global.function
func print(msg) {
}

// @object.class
Calculator := {
  // Adds two numbers
  //
  // Parameters:
  // - a: First number
  // - b: Second number
  //
  // Returns: Sum of a and b
  // @object.method
  add = func(a, b) {
    return a + b
  }
}
```

## Important

* Ignore function names starting with _ or __
