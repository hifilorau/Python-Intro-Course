# Python-Intro-Course

## Chapter 3: Functions

In this chapter, we will explore Python functions, comparing them with JavaScript functions to highlight their similarities and differences. By understanding these concepts, you'll be better equipped to write efficient and clean Python code.

### 3.1 Defining Functions

In Python, functions are defined using the def keyword, followed by the function name, parentheses enclosing the arguments, and a colon to indicate the start of the function body. The function body is indented, and there's no need for curly braces.

In JavaScript:

```
function greet(name) {
  console.log("Hello, " + name + "!");
}
```

```
def greet(name):
    print("Hello, " + name + "!")
```

3.2 Calling Functions

Function calls in Python are similar to those in JavaScript. To call a function, simply use its name followed by parentheses enclosing the arguments.

In JavaScript:

```
greet("Alice");

```

In Python: 
```
greet("Alice")

```

### 3.3 Default Arguments

Python allows you to specify default argument values for functions, which will be used if no value is provided when calling the function. This is similar to JavaScript, but with a different syntax.

In JavaScript:

```
function greet(name = "World") {
  console.log("Hello, " + name + "!");
}
```

In Python: 

```
function greet(name = "World") {
  console.log("Hello, " + name + "!");
}
```

### 3.4 Return Values

To return a value from a function in Python, use the return keyword, just like in JavaScript. The main difference is the lack of semicolons in Python.

In JavaScript:

```
function add(a, b) {
  return a + b;
}
```

In Python: 

```
def add(a, b):
    return a + b

```

### 3.5 Anonymous Functions

Python has a concept similar to JavaScript's anonymous functions, called lambda functions. Lambda functions are small, single-expression functions that can be defined in-line. They are limited in functionality compared to regular functions but can be useful in certain situations.

In JavaScript:

```
const add = (a, b) => a + b;
```

In Python:

```
add = lambda a, b: a + b

```

### 3.6 Variable Scope

Variable scope in Python works similarly to JavaScript. Variables defined within a function have local scope and are not accessible outside the function. Global variables, on the other hand, can be accessed both inside and outside of functions.

In Javascript: 

```
let globalVar = "I'm global!";

function example() {
  let localVar = "I'm local!";
  console.log(globalVar); // Accessible
  console.log(localVar); // Accessible
}

console.log(globalVar); // Accessible
console.log(localVar); // Error: localVar is not defined

```
In Python:

```
global_var = "I'm global!"

def example():
    local_var = "I'm local!"
    print(global_var)  # Accessible
    print(local_var)   # Accessible

print(global_var)  # Accessible
print(local_var)   # Error: local_var is not defined

```

### 3.7 Summary

In this chapter, we discussed Python functions and compared them to JavaScript functions. You learned how to define and call functions, work with default arguments and return values, and use anonymous functions (lambda functions). Additionally, we covered variable scope in both languages.

As you progress through this course, you'll continue to find similarities and differences between Python and JavaScript. These insights will help you become proficient in Python while leveraging your existing JavaScript knowledge. In the next chapter, we will explore conditional statements in Python, further expanding your understanding of the language.
