# Read & Write Files in Python

A file object is: “an object exposing a file-oriented API (with methods such as read() or write()) to an underlying resource.” (Source)

Files on most modern file systems are composed of three main parts:

1.	Header: metadata about the contents of the file (file name, size, type, and so on)
2.	Data: contents of the file as written by the creator or editor
3.	End of file (EOF): special character that indicates the end of the file


There are three different categories of file objects:

•	Text files (_open() will return a TextIOWrapper file object_)

•	Buffered binary files (_open() will return either a BufferedReader or BufferedWriter file object_)

•	Raw binary files (open() will return a FileIO file object)

**Line Endings**

Windows uses the CR+LF characters to indicate a new line

```
Pug\r\n
Jack Russell Terrier\r\n
English Springer Spaniel\r\n
German Shepherd\r\n
```

while Unix and the newer Mac versions use just the LF character.

```
Pug\r
\n
Jack Russell Terrier\r
\n
English Springer Spaniel\r
\n
``` 

**Opening and Closing a File in Python**

_It is your responsibility to close a file after opening it. It’s important_

Including an error: 
``` 
reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()
```

With **with statement**
```
with open('dog_breeds.txt', mode) as reader:
    # Further file processing goes here
```

## Python Exceptions: An Introduction

_ https://realpython.com/python-exceptions/ _

exception error. Is the type of error that occurs whenever syntactically correct Python code results in an error. Python comes with various built-in exceptions as well as the possibility to create self-defined exceptions using the _raise_ keyword. 

```
x = 10
if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))
```

Another idea about raising exceptions, is _asserting_ that a certain value is met: 
``` 
import sys
assert ('linux' in sys.platform), "This code runs on Linux only."
```
Finally, you can use the try-except-else-finally statement. 
