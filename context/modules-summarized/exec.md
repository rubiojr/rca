# Exec Module Summary
Exec module is used to run external commands without invoking the system shell.
## Functions
* exec(args, opts) - Runs command and returns result object
* command(args) - Creates a new command
* look_path(name) - Searches for executable in PATH
## Types
* command - Has path, dir, env, stdout, stderr attributes and run(), output(), combined_output(), start(), wait() methods
* result - Has stdout, stderr, pid attributes

