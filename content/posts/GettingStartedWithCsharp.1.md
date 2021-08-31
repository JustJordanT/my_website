---
title: "Getting started with C# 2/5 - Variables"
cover: images/cover_6.jpeg
coverAlt: "Never Stop Learning"
description: "Getting started with C# 2/5 - Variables"
date: "2021-06-08"
category: "Programming"
tags:
  - programming
  - GettingStartedWithC#
---

## C# Variables

Variables are containers for storing data values.

In C#, there are different types of variables (defined with different keywords), for example:
<!--truncate-->

### int

- stores integers (whole numbers) without decimals, such as 123 or 123.

### double

- stores floating-point numbers, with decimals, such as 19.99 or -19.99.

### char

- stores single characters, such as 'a' or 'B'. Single quotes surround char values

### string

- stores text, such as "Hello World." Double quotes surround string values

### bool

- stores values with two states: true or false

## Declaring Variables

By declaring variables we are creating a variable, you must specify the type and assign it a value:

### Examples

```csharp
int num = 5;
Console.Writeline(num);
```

```csharp
//double
double num = 3.92
Console.Writeline(num);
```

```csharp
string name = "Jordan";
Console.WriteLine(name);
```

### Modifying variables

A good thing to note is if you assign a new value to an existing variable, it will overwrite the previous value:

```csharp
int myNum = 115;
myNum = 220; // myNum is now 220
Console.WriteLine(myNum);
```

### Constants

You can also add the `const` keyword to prevent others from altering the existing values; this could be helpful in certain situations.

```csharp
const int numPi = 3.14
numPi = 20; // error
```

The const keyword is used to tell a variable always to keep the same value.

Note: You cannot declare a constant variable without assigning the value. If you do, an error will occur: A const field requires a value to be provided.

### Using the keyword var.

The `var` keyword has been around for a long time, and it's commonly used in code examples.

The use of the `var` keyword is significant in C#. There are some situations where the data type may be different than the code intended to use it.

```csharp
var message = "Hello world!";

var message = 19.0m;
```

Sneak Peak for the next lesson we will continue to put this all together for what we have learned so far.

```csharp
int age = 25;
int name = "Jordan";

Console.Writeline($"Hey Friends!, my name is {name}, and I am {age}!");
```

If you want to dive in deep with variables take a look at the links below.

### sources

- https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/language-specification/types#default-constructors
- https://docs.microsoft.com/en-us/learn/modules/csharp-literals-variables/
- https://www.w3schools.com/cs/cs_variables.asp

Like, share and follow me 🔥 for more content:

📽[YouTube](https://www.youtube.com/channel/UCWMddXhNGWkzBYYS9cv-7Qg)
☕[Buy me a coffee](https://ko-fi.com/justjordant)
💖[Patreon](https://www.patreon.com/JustJordanT)
🌐[JustJordanT.com](www.justjordant.com)
🐱‍💻[GitHub](https://github.com/JustJordanT)
🤠[Twitter](https://twitter.com/Just_Jordan_T)
🏢[LinkedIn](https://www.linkedin.com/in/justjordant/)