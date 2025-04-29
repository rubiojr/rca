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
