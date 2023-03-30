# Python-Intro-Course

## Chapter 6: Exceptions

In this chapter, we will learn about exceptions in Python and how they compare to error handling in JavaScript. You will learn how to raise exceptions, catch exceptions, and handle errors in Python.

### 6.1 Raising Exceptions

Both Python and JavaScript use the throw keyword to raise exceptions manually. However, Python exceptions are typically instances of the Exception class or its subclasses.

In JavaScript:

```
throw new Error("This is an error message.");

```

In Python:

```
raise Exception("This is an error message.")

```

### 6.2 Catching Exceptions

Python uses the try and except keywords to catch exceptions, whereas JavaScript uses try and catch. The syntax is slightly different, with Python using colons and indentation to define blocks.

In JavaScript:

```
try {
  throw new Error("An error occurred.");
} catch (error) {
  console.error("Caught:", error.message);
}

```

In Python:

```
try:
    raise Exception("An error occurred.")
except Exception as error:
    print("Caught:", error)
```

### 6.3 Handling Multiple Exceptions

Python allows you to catch and handle multiple exception types by specifying multiple except blocks.

In JavaScript:

```
try {
  // Code that may throw different types of errors
} catch (error) {
  if (error instanceof TypeError) {
    console.error("Caught TypeError:", error.message);
  } else if (error instanceof ReferenceError) {
    console.error("Caught ReferenceError:", error.message);
  } else {
    console.error("Caught an unknown error:", error.message);
  }
}

```

In Python:

```
try:
    # Code that may raise different types of exceptions
except TypeError as error:
    print("Caught TypeError:", error)
except ReferenceError as error:
    print("Caught ReferenceError:", error)
except Exception as error:
    print("Caught an unknown error:", error)

```

### 6.4 Finally Clause

Both Python and JavaScript support the finally clause, which contains code that will be executed regardless of whether an exception is raised or not.

In JavaScript:

```
try {
  // Code that may throw an error
} catch (error) {
  console.error("Caught:", error.message);
} finally {
  console.log("This will always run.");
}

```

In Python: 

```
try:
    # Code that may raise an exception
except Exception as error:
    print("Caught:", error)
finally:
    print("This will always run.")
```

### Custon Exceptions

In both Python and JavaScript, you can create custom exceptions by extending built-in exception classes.

In JavaScript:

```
class CustomError extends Error {
  constructor(message) {
    super(message);
    this.name = "CustomError";
  }
}

throw new CustomError("This is a custom error message.");
```

In Python:

```
class CustomError(Exception):
    pass

raise CustomError("This is a custom error message.")
```

### 6.6 Summary

In this chapter, we covered exceptions in Python and compared them to error handling in JavaScript. You learned how to raise exceptions, catch exceptions, handle multiple exceptions, use the finally clause, and create custom exceptions in Python. Understanding the similarities and differences between the two languages will help you become proficient in handling errors in Python.

By completing this course, you now have a good understanding of Python fundamentals. You can confidently write simple programs, use variables and operators, define functions, work with conditional statements, classes, and exceptions. As you continue to practice and apply your new Python skills, you will become more comfortable and proficient in the language.
