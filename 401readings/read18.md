# Automation

## Python Regular Expressions Tutorial

regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not.

Ordinary characters can be used to perform simple exact matches:

```
pattern = r"Cookie"
sequence = "Cookie"
if re.match(pattern, sequence):
    print("Match!")
else: print("Not a match!")
```
PS: the r before the string is called raw string literal.

With the **search** function, you scan through the given string/sequence, looking for the first location where the regular expression produces a match.
The **group** function returns the string matched by the re. You will see both these functions in more detail later.


## shutil — High-level File Operations

The shutil is a module that includes high-level file operations such as copying and archiving.

Copying Files
copyfile() copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file.

Copying File Metadata
By default when a new file is created under Unix, it receives permissions based on the umask of the current user. To copy the permissions from one file to another, use copymode().

Finding Files
The which() function scans a search path looking for a named file. The typical use case is to find an executable program on the shell’s search path defined in the environment variable PATH.

## Automation Ideas

- automatically moving files 
- and renaming them
- open a website with a condition