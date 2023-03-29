# Python-Intro-Course

## Chapter 4: Conditional Statements

In this chapter, we'll explore conditional statements in Python and compare them to their JavaScript counterparts. This will help you better understand how to control the flow of your Python programs using familiar concepts.

### 4.1 If Statements

Python uses the if keyword to create conditional statements, just like JavaScript. However, Python uses colons and indentation instead of curly braces to define code blocks.

In JavaScript:

```
let age = 18;

if (age >= 18) {
  console.log("You are an adult.");
} else {
  console.log("You are a minor.");
}

```
In Python:

```
age = 18

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
    
```

### 4.2 Elif Statements

Python uses the elif keyword (short for "else if") for additional conditions, unlike JavaScript's else if.

In JavaScript:

```
let score = 85;

if (score >= 90) {
  console.log("A");
} else if (score >= 80) {
  console.log("B");
} else if (score >= 70) {
  console.log("C");
} else {
  console.log("F");
}

```
In Python:


```
score = 85

if score >= 90:
    print("A")
elif score >= 80:
    print("B")
elif score >= 70:
    print("C")
else:
    print("F")
```

### 4.3 Ternary Operators

Both Python and JavaScript support ternary operators (also known as conditional expressions) for concise if-else statements.

In JavaScript:

```
let age = 18;
let status = age >= 18 ? "adult" : "minor";
console.log(status);
```

In Python:

```
age = 18
status = "adult" if age >= 18 else "minor"
print(status)
```

### 4.4 While Loops

Python and JavaScript both use the while keyword for while loops. As with if statements, Python uses colons and indentation instead of curly braces.

In JavaScript:

```
let i = 0;

while (i < 5) {
  console.log(i);
  i++;
}

```

In Python:

```
i = 0

while i < 5:
    print(i)
    i += 1
    
```

### 4.5 For Loops

Python has a different syntax for iterating over sequences (such as lists or strings) using the for keyword. Instead of using an index variable, Python uses the in keyword to iterate directly over the items in a sequence.

In JavaScript:

```
let numbers = [1, 2, 3, 4, 5];

for (let i = 0; i < numbers.length; i++) {
  console.log(numbers[i]);
}
```

In Python:

```
numbers = [1, 2, 3, 4, 5]

for number in numbers:
    print(number)
```

### 4.6 Summary

In this chapter, we covered conditional statements in Python and compared them to those in JavaScript. You learned how to use if statements, elif statements, ternary operators, while loops, and for loops in Python, all while leveraging your existing JavaScript knowledge. By understanding the similarities and differences between the two languages, you'll be better equipped to write efficient and clean Python code.

In the next chapter, we'll dive into Python classes, further expanding your Python skillset and deepening your understanding of the language.
