<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Python Print Function</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #1e1e1e;
            color: #dcdcdc;
            padding: 20px;
        }
        code {
            background-color: #2e2e2e;
            padding: 2px 4px;
            border-radius: 4px;
        }
        pre {
            background-color: #2e2e2e;
            padding: 10px;
            border-radius: 4px;
            overflow-x: auto;
        }
        h2 {
            color: #dca3a3;
        }
        a {
            color: #efefef;
        }
    </style>
</head>
<body>
    <h1>Python Print Function</h1>
    <p>The <code>print</code> function in Python is used to display output to the console. It can take various parameters to customize the output.</p>

    <h2>Syntax</h2>
    <p>The basic syntax of the <code>print</code> function is:</p>
    <pre><code>print(*objects, sep=' ', end='\n', file=sys.stdout, flush=False)</code></pre>

    <h2>Parameters</h2>
    <ul>
        <li><code>*objects</code>: Any number of objects to be printed. They are converted to strings and separated by <code>sep</code>.</li>
        <li><code>sep</code>: A string inserted between the objects. Default is a space (' ').</li>
        <li><code>end</code>: A string appended after the last object. Default is a newline ('\n').</li>
        <li><code>file</code>: A file-like object (stream) to which the output is printed. Default is <code>sys.stdout</code>.</li>
        <li><code>flush</code>: A boolean specifying whether to forcibly flush the stream. Default is <code>False</code>.</li>
    </ul>

    <h2>Examples</h2>

    <h3>Basic Example</h3>
    <pre><code>print("Hello, World!")</code></pre>
    <p>Output:</p>
    <pre><code>Hello, World!</code></pre>

    <h3><code>sep</code> Parameter</h3>
    <p>The <code>sep</code> parameter specifies the separator between multiple objects:</p>
    <pre><code>print("Hello", "World", sep="-")</code></pre>
    <p>Output:</p>
    <pre><code>Hello-World</code></pre>

    <h4>More Examples with <code>sep</code></h4>
    <pre><code>print("apple", "banana", "cherry", sep=", ")
print("2021", "09", "30", sep="/")
print("Name:", "Alice", "Age:", "30", sep=" | ")</code></pre>
    <p>Outputs:</p>
    <pre><code>apple, banana, cherry
2021/09/30
Name: | Alice | Age: | 30</code></pre>

    <h3><code>end</code> Parameter</h3>
    <p>The <code>end</code> parameter specifies what to print at the end. By default, it is a newline:</p>
    <pre><code>print("Hello", end=" ")
print("World")</code></pre>
    <p>Output:</p>
    <pre><code>Hello World</code></pre>

    <h4>More Examples with <code>end</code></h4>
    <pre><code>print("Loading", end="...")
print("Done!")

for i in range(3):
    print(i, end=" ")</code></pre>
    <p>Outputs:</p>
    <pre><code>Loading...Done!
0 1 2 </code></pre>

    <h3><code>file</code> Parameter</h3>
    <p>The <code>file</code> parameter specifies the file-like object to which the output is printed:</p>
    <pre><code>with open('output.txt', 'w') as f:
    print("Hello, World!", file=f)</code></pre>
    <p>This writes "Hello, World!" to the file <code>output.txt</code>.</p>

    <h4>More Examples with <code>file</code></h4>
    <pre><code>import sys
print("Error message", file=sys.stderr)

with open('log.txt', 'a') as f:
    print("Logging information", file=f)</code></pre>
    <p>This writes "Logging information" to the file <code>log.txt</code> in append mode and "Error message" to the standard error stream.</p>

    <h3><code>flush</code> Parameter</h3>
    <p>The <code>flush</code> parameter forces the output stream to be flushed:</p>
    <pre><code>print("Hello, World!", flush=True)</code></pre>
    <p>This ensures that the output is immediately flushed, useful for real-time applications.</p>

    <h4>More Examples with <code>flush</code></h4>
    <pre><code>import time
for i in range(3):
    print(i, flush=True)
    time.sleep(1)</code></pre>
    <p>This prints the numbers 0, 1, and 2 with a 1-second delay between each, ensuring each number is immediately printed.</p>

</body>
</html>
