# Filepath Module Summary
Filepath module provides utilities to manipulate file paths with OS-specific separators.
## Functions
* abs(path) - Returns absolute representation of path
* base(path) - Returns last element of path
* clean(path) - Returns shortest path name equivalent
* dir(path) - Returns all but last element of path
* ext(path) - Returns file extension
* is_abs(path) - Checks if path is absolute
* join(paths...) - Joins path elements with OS-specific separator
* match(pattern, name) - Checks if filename matches shell pattern
* rel(basepath, targpath) - Returns relative path from base to target
* split_list(path) - Splits path into directory and file components as list
* split(path) - Splits path into directory and file components
* walk_dir(root, fn) - Walks file tree calling function for each entry
