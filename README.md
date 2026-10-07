# Learning C#

Repository for learning **C#** programming fundamentals, concepts, and practice exercises.

This guide covers the **core basics** you need to get started with C#. Work through each section in order, write small programs for every topic, and practice regularly.

---

## 1. Setup & First Program
- Install .NET SDK (latest LTS version recommended)
- Install an IDE / editor (Visual Studio, VS Code + C# Dev Kit, Rider)
- Understand the .NET ecosystem (runtime, libraries, tools)
- Create and run your first console app (`dotnet new console`)
- Basic `dotnet` CLI commands (`build`, `run`, `add package`)

---

## 2. Basic Syntax & Structure
- Comments (`//`, `/* */`, and XML documentation comments)
- Namespaces and `using` directives
- The `Main` method / top-level statements
- Statements, expressions, and the semicolon
- Code style and naming conventions (PascalCase, camelCase)

---

## 3. Variables, Data Types & Constants
- Value types: `int`, `long`, `float`, `double`, `decimal`, `bool`, `char`
- Reference types introduction (`string`, `object`)
- Variable declaration and initialization
- `const` and `readonly`
- Implicit typing with `var`
- Type conversion / casting (`Convert`, `Parse`, `TryParse`)
- Nullable value types (`int?`)

---

## 4. Input & Output
- `Console.WriteLine` and `Console.Write`
- `Console.ReadLine`
- String interpolation (`$"..."`)
- Basic formatting
- Reading and converting user input safely

---

## 5. Operators
- Arithmetic operators
- Relational / comparison operators
- Logical operators (`&&`, `||`, `!`)
- Assignment and compound assignment operators
- Increment / decrement
- Null-coalescing operator (`??`)
- Null-conditional operator (`?.`)

---

## 6. Control Flow
- `if`, `else if`, `else`
- `switch` statements and switch expressions
- Ternary operator
- `for`, `foreach`, `while`, `do-while` loops
- `break`, `continue`, and `return`
- Pattern matching basics (introduction)

---

## 7. Methods (Functions)
- Method declaration and definition
- Parameters and return types
- Pass by value vs `ref` / `out` / `in`
- Method overloading
- Optional and named parameters
- Local functions
- Expression-bodied members

---

## 8. Arrays, Lists & Strings
- Single and multidimensional arrays
- `System.Array` methods
- `List<T>` (generic collections)
- `string` immutability and common methods
- StringBuilder (introduction)
- `foreach` with collections

---

## 9. Object-Oriented Programming (Basics)
- Classes and objects
- Fields, properties (auto-properties), and methods
- Access modifiers (`public`, `private`, `protected`, `internal`)
- Constructors
- `this` keyword
- Encapsulation
- Static members

---

## 10. Inheritance & Polymorphism (Introduction)
- Inheritance (`:`)
- `base` keyword
- Method overriding (`virtual` / `override`)
- Abstract classes and methods (basics)
- Interfaces (introduction)
- Polymorphism in practice

---

## 11. Exception Handling
- `try` / `catch` / `finally`
- Common exception types
- Throwing exceptions (`throw`)
- Custom exceptions (introduction)
- Best practices for error handling

---

## 12. Collections & Generics (Basics)
- Why generics matter
- `List<T>`, `Dictionary<TKey, TValue>`, `HashSet<T>`
- Iterating collections
- Basic LINQ introduction (`Where`, `Select`, `FirstOrDefault`)

---

## 13. File I/O (Basics)
- Reading and writing text files
- `File`, `FileInfo`, `StreamReader`, `StreamWriter`
- Working with paths (`Path` class)
- Simple JSON serialization (introduction with `System.Text.Json`)

---

## 14. Debugging & Tooling
- Using the debugger in Visual Studio / VS Code
- Breakpoints, watch windows, call stack
- Common runtime exceptions and how to diagnose them
- NuGet package management basics

---

## 15. Good Practices for Beginners
- Follow C# naming conventions
- Prefer properties over public fields
- Use meaningful names
- Keep methods small and focused
- Handle nulls safely
- Write readable code first, optimize later
- Practice solving small problems daily

---

## Suggested Learning Path
1. Complete sections 1–6 thoroughly
2. Practice with console applications (calculators, quizzes, simple games)
3. Master methods, arrays/lists, and strings
4. Learn classes and basic OOP
5. Add inheritance, interfaces, and exception handling
6. Build small projects (todo app, simple inventory system, text adventure)

---

## Resources (Recommended)
- **Official**: Microsoft Learn – C# documentation and tutorials
- **Books**: *C# 12 and .NET 8 – Modern Cross-Platform Development* (Mark J. Price), *C# in a Nutshell*
- **Online**: learn.microsoft.com, csharp.net, DotNetPerls
- **Practice**: LeetCode (Easy), HackerRank C#, Exercism C# track

---

Happy coding!  
Focus on understanding concepts deeply and writing clean, readable code.
