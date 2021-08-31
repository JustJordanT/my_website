---
title: "Getting started with C# 3/5 - String Formatting"
cover: images/cover_6.jpeg
coverAlt: "Never Stop Learning"
description: "Getting started with C# 3/5 - String Formatting"
date: "2021-06-09"
category: "Programming"
tags:
  - programming
  - GettingStartedWithC#
---
Hey friends, today I will show you how string formatting works in C#; let's dive in.

You can follow long with your own code or clone the git repo as well. [gettingStartedWIthCsharp - stringFormatting](https://github.com/JustJordanT/gettingStartedWithCsharp/tree/main/gettingStartedWIthCsharp%20-%20stringFormatting/stringFormat)
<!--truncate-->

### Learn By Doing.

All right, so let's learn a little .NET CLI as well; we start by making a new .NET project. Now let's create our .NET project.

```cSharp
//The following will create our console app in the directory, in the string Format.
dotnet new console -o stringFormat
```

This basic console app for now, and we will be adding upon this. Here our `Main` method will be asking for your first and last name, and then it will give you your initials.

```csharp
using System;

namespace string format
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Enter you first name: ").IsUpper;
            string firstName = Console.ReadLine();

            Console.WriteLine("Enter you last name: ");
            string lastName = Console.ReadLine();

            Console.WriteLine($"Your initials are: '{firstName[0]}.{lastName[0]}'");
        }
    }
}
```

### string interpolation

If we look at the existing code block that we just ran, we can see that the final line seems a little different from a standard print string. This is called `string interpolation`; this is a way of formatting our output; we can add the `$"" ` to our write lines to call variables from directly in the `Console.WriteLine()` method.

```cSharp
Console.WriteLine($"Your initials are: '{firstName[0]}.{lastName[0]}'");
```


### String Indexes

You can access the characters in a string by referring to its index number inside square brackets `[]`. If we take a look at our example, we can see that we already used this to get the first character from our first and the last name gets it our initials.
```csharp
Console.WriteLine($"Your initials are: '{firstName[0]}.{lastName[0]}'");
```

Okay, now let's look at a few other methods that can help us format our stings.

### ToUpper()

This is a method that you can add to your strings to make sure that you always get upper case lettering no matter what the user puts in. If we take a tool at the following code block, we can see that we need to add some extra variables to our method. If we look at our new variables, we can see that we call the `ToUpper()` method when it's attached to an existing variable. ie `fistName.ToUpper()`

**Side Note**
C# is a strongly typed language which means, you must declare a variable type before you can use it. We see that with both the variables, we are calling the types we want to use. The "var" keyword is used to declare a var type variable. The var type variable can be used to store a simple .NET data type, a complex type, an anonymous type, or a user-defined type.
From a programming standpoint, you can think of `var == string, double, int, char, bool, long, object`.


```cSharp
Console.WriteLine("Enter you first name: ");
            string firstName = Console.ReadLine();
            var upperFirstName = firstName.ToUpper();

            Console.WriteLine("Enter you lastname: ");
            string lastName = Console.ReadLine();
            var upperLastName = lastName.ToUpper();

            Console.WriteLine($"Your initials are: '{upperFirstName[0]}.{upperLastName[0]}'");
```

## Summary

We can see that in this session, we were able to complete the following.

1. Being able to create variables.
2. Taking input from the console.
3. Apply indexing to our outputs to get only certain characters.
4. Using different types.
5. Formatting methods.
6. Using string interpolation to format our output.

## Conclusion

Formatting strings can be instrumental in `real-world` scenarios; this could range from formatting numbers for security reasons or validating that the data that is being used is only received in a specific format itself.
Here is some homework for you. Are you able to find any other method that we can use to format our data? I will give you one more to look into to, `.ToLower` the name gives it away if you have made it this far; with this, we can turn all our data into a lower casing format. Explore and see what other methods you can find as well.


## Resources

- [How To Format Strings In C#](https://www.c-sharpcorner.com/UploadFile/mahesh/format-string-in-C-Sharp/)
- [w3schools](https://www.w3schools.com/cs/index.php)
- [What Does “var” Mean In C#?](https://www.c-sharpcorner.com/article/what-does-var-mean-in-c-sharp/)
- [$ - string interpolation (C# reference)](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/tokens/interpolated)

Like, share and follow me 🔥 for more content:

📽[YouTube](https://www.youtube.com/channel/UCWMddXhNGWkzBYYS9cv-7Qg)
☕[Buy me a coffee](https://ko-fi.com/justjordant)
💖[Patreon](https://www.patreon.com/JustJordanT)
🌐[JustJordanT.com](www.justjordant.com)
🐱‍💻[GitHub](https://github.com/JustJordanT)
🤠[Twitter](https://twitter.com/Just_Jordan_T)
🏢[LinkedIn](https://www.linkedin.com/in/justjordant/)

Get out there and build and happy coding.