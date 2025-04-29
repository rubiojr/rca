# regexp Module Summary
The regexp module provides regular expression matching functionality using Go's regexp syntax.
## Functions
- `compile(expr string)` - Compiles a regular expression string
- `match(expr, s string)` - Tests if a string contains a pattern match
## Types
- `regexp` - Represents a compiled regular expression
- `match(s string)` - Tests if string contains pattern match
- `find(s string)` - Returns leftmost match
- `find_all(s string)` - Returns all matches
- `find_submatch(s string)` - Returns matches and submatches
- `replace_all(s, repl string)` - Replaces all matches with replacement
- `split(s string)` - Splits string by pattern matches
