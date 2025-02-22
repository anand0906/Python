<h1>print</h1>
<p>print is a built-in function in python which is used to display the output data on console.</p>
<p>It is one of the most frequently used functions and is essential for displaying information, debugging code, and interacting with users.</p>
<p><strong>Syntax</strong></p>
<p>The basic syntax of the print function is:</p>

```python
print(*objects, sep=' ', end='\n', file=sys.stdout, flush=False)
```

<ul>
	<li><strong>*objects : </strong> Any number of objects (strings, numbers, variables, etc.) to be printed.</li>
	<li><strong>sep : </strong> A string inserted between objects. The default is a space (' ')</li>
	<li><strong>end : </strong> A string appended after the last object. The default is a newline ('\n')</li>
	<li><strong>file : </strong> An object with a write method, defaulting to sys.stdout (usually the console)</li>
	<li><strong>flush : </strong> A boolean specifying whether to forcibly flush the stream (immediatly adding data to file). The default is False</li>
</ul>

<h3>sep</h3>
<p>The sep parameter specifies the separator between multiple objects. By default, it is a space (' ').</p>

```python
print("apple", "banana", "cherry", sep=", ")

#output : apple, banana, cherry

print("apple", "banana", "cherry", sep="-")

#output : apple-banana-cherry

print(1, 2, 3, sep="")

#output : 123

print(2,"banana",3,"cherry",sep=":")

#output : 2:banana:3:cherry

print(2,"banana",3,"cherry",sep=1)

#output : sep must be None or a string, not int
```

<h3>end</h3>
<p>The end parameter specifies what to print at the end of the output. By default, it is a newline ('\n').</p>

```python
print("Hello", end=" ")
print("World")

#output: Hello World

print("Hello")
print("World")

#output : Hello 
#         World

print(1,end="")
print(2)

#output : HelloWorld

print(1,2,3,end=2)

#output : TypeError: end must be None or a string, not int         
```

<h3>file</h3>
<p>The file parameter allows you to redirect the output from the console to a file or any object that has a write method. This parameter gives you flexibility in where your output is directed, beyond just printing to the console.</p>
<p><strong>file : </strong>specifies the output destination. By default, it is sys.stdout, which represents the console (standard output).</p>
<p><strong>Examples</strong></p>
<h6>Printing to a File</h6>
<p>To print output directly to a file, you open the file in write mode ("w"), and pass the file object as the file parameter to print.</p>

```python
# Open a file in write mode
with open("output.txt", "w") as file:
    print("Hello, World!", file=file)
```

<ul>
	<li>open("output.txt", "w") opens the file output.txt in write mode ("w").</li>
	<li>'with' statement ensures the file is properly closed after use.</li>
	<li>print("Hello, World!", file=file) prints "Hello, World!" to output.txt.</li>
</ul>

<h6>Appending to a File</h6>
<p>You can also append to a file by opening it in append mode ("a"):</p>

```python
# Append to an existing file
with open("output.txt", "a") as file:
    print("This is an appended line.", file=file)
```

<ul>
	<li>open("output.txt", "a") opens output.txt in append mode ("a").</li>
	<li>print("This is an appended line.", file=file) appends the line to output.txt.</li>
</ul>

<h6>Using sys.stderr for Error Messages</h6>
<p>You can redirect errors or other messages to sys.stderr, which is typically used for error output:</p>

```python
import sys

try:
    result = 10 / 0  # Raises a ZeroDivisionError
except ZeroDivisionError as e:
    print(f"Error occurred: {e}", file=sys.stderr)

```

<p>print(f"Error occurred: {e}", file=sys.stderr) prints the error message to sys.stderr, which is the standard error stream.</p>
