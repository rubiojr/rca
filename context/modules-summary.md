# Errors Module Summary
Errors module provides functions for creating error values in Risor.
## Functions
* new(string) - Creates a new error value with the given message

# Exec Module Summary
Exec module is used to run external commands without invoking the system shell.
## Functions
* exec(args, opts) - Runs command and returns result object
* command(args) - Creates a new command
* look_path(name) - Searches for executable in PATH
## Types
* command - Has path, dir, env, stdout, stderr attributes and run(), output(), combined_output(), start(), wait() methods
* result - Has stdout, stderr, pid attributes

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
# HTTP Module Summary
HTTP module provides functions for making HTTP requests and handling responses.
## Functions
* get(url, headers, params) - Creates a GET request
* delete(url, headers, params) - Creates a DELETE request
* head(url, headers, params) - Creates a HEAD request
* listen_and_serve(addr, handler) - Starts an HTTP server
* listen_and_serve_tls(addr, cert_file, key_file, handler) - Starts an HTTPS server
* patch(url, headers, body) - Creates a PATCH request
* post(url, headers, body) - Creates a POST request
* put(url, headers, body) - Creates a PUT request
* request(url, options) - Creates a custom HTTP request
## Types
* request - Has url, content_length, header attributes and send(), add_header(), add_cookie(), set_body(), set_data() methods
* response - Has status, status_code, proto, content_length, header, cookies, response attributes and json(), text(), close() methods
* response_writer - Has add_header(), del_header(), write(), write_header() methods
# Math Module Summary
Math module provides constants and mathematical functions, wrapping Go's math package with additional utilities.
## Constants
* PI - Mathematical constant pi (3.141592653589793)
* E - Mathematical constant e (2.718281828459045)
## Functions
* abs(x) - Returns absolute value
* sqrt(x) - Returns square root
* min(x, y) - Returns smaller of two numbers
* max(x, y) - Returns larger of two numbers
* floor(x) - Returns largest integer less than or equal to x
* ceil(x) - Returns smallest integer greater than or equal to x
* sin(x) - Returns sine
* cos(x) - Returns cosine
* tan(x) - Returns tangent
* mod(x, y) - Returns remainder of division
* log(x) - Returns natural logarithm
* log10(x) - Returns base-10 logarithm
* log2(x) - Returns base-2 logarithm
* pow(x, y) - Returns x raised to power of y
* pow10(x) - Returns 10 raised to power of x
* is_inf(x) - Checks if value is infinity
* inf() - Returns infinite value
* round(x) - Rounds to nearest integer
* sum(list) - Returns sum of all numbers in list
# OS Module Summary
OS module provides platform-independent access to operating system functionality.
## Attributes
* stdin - Standard input file pointer
* stdout - Standard output file pointer
## Functions
* chdir(dir) - Changes working directory
* create(name) - Creates or truncates a file
* environ() - Returns environment variables as list of strings
* exit(code) - Terminates program with exit code
* getenv(key) - Gets environment variable value
* getpid() - Returns current process ID
* getuid() - Returns current user ID
* getwd() - Gets current working directory
* hostname() - Returns system hostname
* mkdir_all(path, perm) - Creates directory with parents
* mkdir_temp(dir, prefix) - Creates temporary directory
* mkdir(path, perm) - Creates directory
* open(name) - Opens file for reading
* read_dir(name) - Lists directory contents
* read_file(name) - Reads file contents
* remove(name) - Removes file or empty directory
* remove_all(name) - Removes directory and contents
* rename(old, new) - Renames/moves file or directory
* setenv(key, value) - Sets environment variable
* stat(name) - Returns file information
* symlink(old, new) - Creates symbolic link
* temp_dir() - Returns temporary directory path
* unsetenv(key) - Unsets environment variable
* user_cache_dir() - Returns user cache directory
* user_config_dir() - Returns user config directory
* user_home_dir() - Returns user home directory
* write_file(name, data) - Writes data to file
## Types
* File - Has read(), write(), close() methods
* FileInfo - Contains name, mode, size, mod_time attributes
* DirEntry - Contains name, type attributes
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
# Strings Module Summary
String manipulation functions from the Go standard library.
## Functions
* compare(s1, s2) - Compares strings lexicographically
* contains(s, substr) - Checks if string contains substring
* count(s, substr) - Counts non-overlapping instances of substring
* fields(s) - Splits string on whitespace
* has_prefix(s, prefix) - Checks if string starts with prefix
* has_suffix(s, suffix) - Checks if string ends with suffix
* index(s, substr) - Returns first index of substring or -1
* join(a, sep) - Concatenates strings with separator
* last_index(s, substr) - Returns last index of substring or -1
* repeat(s, count) - Creates new string with repeated copies
* replace_all(s, old, new) - Replaces all instances of old with new
* split(s, sep) - Splits string on separator
* to_lower(s) - Converts string to lowercase
* to_upper(s) - Converts string to uppercase
* trim_prefix(s, prefix) - Removes leading prefix if present
* trim_space(s) - Removes leading and trailing whitespace
* trim_suffix(s, suffix) - Removes trailing suffix if present
* trim(s, cutset) - Removes leading and trailing characters in cutset
# Time Module Summary
Time module provides functionality for measuring and displaying time.
## Constants
* ANSIC, UnixDate, RubyDate, RFC822, RFC822Z, RFC850, RFC1123, RFC1123Z, RFC3339, RFC3339Nano, Kitchen, Stamp, StampMilli, StampMicro, StampNano - Predefined date/time formats
## Functions
* now() - Returns current time
* unix(sec, nsec) - Returns time from Unix timestamp
* parse(layout, value) - Parses string into time object
* since(t) - Returns seconds elapsed since given time
* sleep(duration) - Pauses execution for specified seconds
## Types
* time - Has before(t), after(t), format(layout), utc(), unix() methods
