# LinuxShell

## Special Variables
* $0: Shell script name
* $1, $2, ..., $N : The first, second, ..., Nth argument
* $#: Number of Arguments. # usually represents Number.
* $@: All aguments. @ -> a -> all
* $$: Process ID
* $?: Exit Code

## Quotes
* Single Quote('): Nothing gets expanded, like raw string
* Double Quote("): Like single quote but expand any variables appear within double quotes.

## Condition tests
There are three general categories of test operations:
* file tests
* string tests
* arithmetic tests

### File Tests

* -e : Returns true if a file exists
* -s : Returns true if a file is not empty
* -nt: Newer than, [file1 -nt file2 ], returns true if file is newer than file2
* -ot: Older than
* -ef: Compare two files and returns true if they share inode numbers and devices

#### File Type Operators
* -f : Returns true if it's a regular file
* -d : Returns true if it's a directory
* -h: Symbolic link
* -b : Block device
* -c : Character device
* -p : Named pipe
* -S : Socket

#### File Permissions Operators
* -r : Readable
* -w : Writable
* -x : Executable
* -u : Setuid
* -g : Setgid
* -k : "Sticky"

### String Tests
* -z : Returns true if it's empty string
* -n : Returns true if not empty string

### Arithmetic Tests
equal sign (=) looks for *string* equality, NOT numberic equality.
* -eq : Equal to
* -ne : Not equal to
* -lt : Less than
* -gt : Greater than
* -le : Less than or equal to
* -ge : Greater than or equal to

