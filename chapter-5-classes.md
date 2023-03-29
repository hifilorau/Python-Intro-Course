# Python-Intro-Course

## Chapter 5: Classes

In this chapter, we'll delve into Python classes and compare them with JavaScript classes. By understanding the similarities and differences between the two, you'll be better equipped to create and work with object-oriented code in Python.

### 5.1 Defining Classes

Python classes are defined using the class keyword, similar to JavaScript. However, Python uses colons and indentation instead of curly braces for defining the class body. The __init__ method in Python is equivalent to the constructor function in JavaScript.

In JavaScript:

```
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log("Hello, my name is " + this.name + ".");
  }
}

```
In Python:

```
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def greet(self):
        print("Hello, my name is " + self.name + ".")
```

### 5.2 Creating Objects

To create an object (instance) of a class, both Python and JavaScript use the class name followed by parentheses enclosing the arguments for the constructor.

In JavaScript:

```
let alice = new Person("Alice", 30);
```
In Python:

```
alice = Person("Alice", 30)
```

### 5.3 Accessing Properties and Methods

Python and JavaScript have similar syntax for accessing object properties and methods.

In JavaScript:

```
console.log(alice.name); // Output: Alice
alice.greet(); // Output: Hello, my name is Alice.
```

In Python:

```
print(alice.name)  # Output: Alice
alice.greet()  # Output: Hello, my name is Alice.

```

### 5.4 Inheritance

Both Python and JavaScript support inheritance, allowing you to create subclasses that inherit properties and methods from their parent classes. The syntax for defining subclasses and invoking parent class constructors is slightly different between the two languages.

In JavaScript:

```
class Employee extends Person {
  constructor(name, age, title) {
    super(name, age);
    this.title = title;
  }

  introduce() {
    super.greet();
    console.log("I work as a " + this.title + ".");
  }
}
```

In Python:

class Employee(Person):
    def __init__(self, name, age, title):
        super().__init__(name, age)
        self.title = title

    def introduce(self):
        super().greet()
        print("I work as a " + self.title + ".")

### 5.5 Summary

In this chapter, we explored Python classes and compared them with JavaScript classes. You learned how to define classes, create objects, access properties and methods, and work with inheritance in Python, building on your existing JavaScript knowledge. Understanding the similarities and differences between the two languages will help you become proficient in writing object-oriented Python code.

In the next chapter, we'll discuss exceptions in Python, further expanding your understanding of the language and its error handling mechanisms.


