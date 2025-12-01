# Explicode

![Download Extension](https://marketplace.visualstudio.com/items?itemName=Explicode.explicode)

Explicode revolutionizes the way you document code by allowing you to write **rich Markdown documentation directly alongside your implementation**, just like Overleaf does for LaTeX. Since the documentation lives inside **comments**, it does **not affect your code** and works with **any programming language**.  

By keeping the docs in the code rather than in external files, updating and collaborating becomes seamless—**version control works the same way as your code with Git**. Explicode lets you open a live preview on the right side of your editor, rendering both code and Markdown in real time.  

You can add **headers, text styling, math, and images**, making it ideal for **academia, open source projects, and math-heavy repositories** like AI/ML. Finally, your documentation can be **exported as Markdown or HTML** for sharing or publishing.

![GIF](demo.gif)

---

## Supported Languages

Python, JavaScript, TypeScript, JavaScript React, TypeScript React, Java, C++, C, C#, Rust, Go, Ruby, PHP, Swift, Kotlin, Julia, MATLAB, Scala, Dart, CSS, SCSS, LESS, SQL, Lua, Perl, LaTeX, Elixir, Elm, CoffeeScript, Objective-C.

> **Note:** Please contact us if you would like another language supported, or if you encounter issues with specific comment syntax.

---

## Quick Guide

You can create Markdown documentation in several ways:

- Press `Control+Alt+M` to add a Markdown block.  
- Right-click and select **Inject Markdown**.  
- Manually enter multi-line comments with the tags `@startmd` and `@endmd`. 

Markdown syntax inside these tags will be automatically highlighted.

#### Example for Python

```python
''' @startmd
# Fibonacci
- `Input`: n (int) — Number of Fibonacci numbers to generate.
- `Output`: List of the first n Fibonacci numbers.
@endmd '''

def fibonacci(n):
    if n <= 0:
        return []
    elif n == 1:
        return [0]
    seq = [0, 1]
    for _ in range(2, n):
        seq.append(seq[-1] + seq[-2])
    return seq

fibonacci(5)  # Output: [0, 1, 1, 2, 3]
```

#### Example for JavaScript:

```javascript
/* @startmd
# Fibonacci
- `Input`: n (int) Number of Fibonacci numbers to generate.
- `Output`: List of first n Fibonacci numbers.
@endmd */

function fibonacci(n) {
    if (n <= 0) return [];
    if (n === 1) return [0];

    const seq = [0, 1];
    for (let i = 2; i < n; i++) {
        seq.push(seq[i - 1] + seq[i - 2]);
    }
    return seq;
}

fibonacci(5)  // Output: [0, 1, 1, 2, 3]
```

Use `Control+Alt+E` or right click `Open with Explicode` to open live rendered preview on the right window. 

---

## Supported Markdown Syntax

[Markdown Guide](https://www.markdownguide.org/basic-syntax/)

## Contact

Please email froem076@umn.edu with new feature ideas, bugs, and collaboration.
