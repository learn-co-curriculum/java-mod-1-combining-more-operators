# String Concatenation

## Learning Goals

- Explain how to concatenate `String` values with the `+` operator

## Introduction

Earlier, we learned that an expression returns value, and we learned about the
`+` operator in the context of numbers. Let's now expand both our understanding
of expressions and of the `+` operator.

## Combining Operator

The `+` operator can apply to text in Java. For example:

```java
String greeting = "Hello, ";
String name = "Maggie";
String message = greeting + name;
```

This would result in the variable `message` holding the value "Hello, Maggie".
For variables of type `String`, the `+` operator concatenates both sides of the
operator.

Now consider the following statement:

```java
System.out.println(greeting + name);
```

The expression `greeting + name` returns the value "Hello, Maggie", which is
then passed to the `println()` method, which prints it on the screen.

The `println()` method knows how to handle data types other than `String`
too! For example:

```java
boolean trueVar = true;
boolean falseVar = false;
System.out.println(trueVar);
```

The above code snippet will print "true" on the screen.

And since `trueVar && falseVar` is an expression that returns a `boolean`, we
can actually pass that expression to the `println()` method:

```java
boolean trueVar = true;
boolean falseVar = false;
System.out.println(trueVar && falseVar);
```

This will output "false" on the screen.

Combining everything we've learned in this section, we can actually create the
following statements:

```java
boolean trueVar = true;
boolean falseVar = false;
System.out.println("true && false = " + (trueVar && falseVar));
```

Which will output the following:

```plaintext
true && false = false
```
