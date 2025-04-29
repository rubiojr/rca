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
