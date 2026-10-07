# 2. Basic Syntax & Structure

## Goal
Understand the fundamental building blocks of a C# program.

---

## 2.1 Comments

```csharp
// Single-line comment

/* 
   Multi-line
   comment
*/

/// <summary>
/// XML documentation comment (used by IntelliSense and tools)
/// </summary>
```

---

## 2.2 Namespaces and `using`

```csharp
using System;
using System.Collections.Generic;

namespace MyApp
{
    class Program
    {
        static void Main()
        {
            Console.WriteLine("Hello");
        }
    }
}
```

With **file-scoped namespaces** (C# 10+):

```csharp
namespace MyApp;

class Program
{
    // ...
}
```

---

## 2.3 Top-Level Statements

Modern C# allows you to write code directly in `Program.cs` without a class or `Main` method:

```csharp
Console.WriteLine("Hello from top-level statements!");
```

The compiler generates the necessary boilerplate for you.

---

## 2.4 Statements & Expressions

- A **statement** is a complete instruction ending with `;`
- An **expression** produces a value

```csharp
int x = 5 + 3;               // statement containing an expression
Console.WriteLine(x);        // statement
```

---

## 2.5 Naming Conventions (Very Important in C#)

| Element              | Convention       | Example                |
|----------------------|------------------|------------------------|
| Classes, Methods, Properties | PascalCase     | `PlayerHealth`, `CalculateDamage` |
| Local variables, parameters  | camelCase      | `playerHealth`, `damage` |
| Constants            | PascalCase       | `MaxHealth`            |
| Private fields       | _camelCase or camelCase | `_health` or `health` |

C# community takes naming conventions seriously — follow them from the start.

---

## 2.6 Code Style Tips

- Use 4 spaces for indentation
- Opening brace `{` on the same line or next line (both are accepted, stay consistent)
- One statement per line
- Keep lines reasonably short

---

## Practice
1. Write a program using both single-line and multi-line comments.
2. Try both classic `Main` style and top-level statements.
3. Experiment with different naming styles and see how IntelliSense reacts.

---

## Next Step
→ [03. Variables, Data Types & Constants](03-variables-data-types-and-constants.md)
