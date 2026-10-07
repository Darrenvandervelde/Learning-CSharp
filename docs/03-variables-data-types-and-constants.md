# 3. Variables, Data Types & Constants

## Goal
Learn how to store and work with data in C#.

---

## 3.1 Common Value Types

| Type      | Size     | Example              | Notes                     |
|-----------|----------|----------------------|---------------------------|
| `int`     | 4 bytes  | `42`                 | Most common integer       |
| `long`    | 8 bytes  | `42L`                | Large integers            |
| `float`   | 4 bytes  | `3.14f`              | Single precision          |
| `double`  | 8 bytes  | `3.14159`            | Double precision (default)|
| `decimal` | 16 bytes | `19.99m`             | High precision (money)    |
| `bool`    | 1 byte   | `true` / `false`     |                           |
| `char`    | 2 bytes  | `'A'`                | Unicode character         |

---

## 3.2 Declaring and Initializing Variables

```csharp
int age = 25;
double price = 19.99;
bool isActive = true;
char grade = 'A';
string name = "Darren";          // reference type

var score = 100;                 // type inferred as int
```

`var` is very common in modern C# when the type is obvious.

---

## 3.3 Constants

```csharp
const double Pi = 3.14159;       // Must be known at compile time

readonly int MaxPlayers = 4;     // Can be set in constructor
```

---

## 3.4 Nullable Value Types

```csharp
int? optionalAge = null;         // Can hold null

if (optionalAge.HasValue)
{
    Console.WriteLine(optionalAge.Value);
}

// Null-coalescing
int age = optionalAge ?? 0;
```

---

## 3.5 Type Conversion

```csharp
// Implicit
int x = 10;
double y = x;

// Explicit (casting)
double pi = 3.14159;
int approx = (int)pi;            // 3

// Safer conversion methods
int number = Convert.ToInt32("42");
int.TryParse("42", out int result);   // preferred for user input
```

---

## 3.6 String is a Reference Type

```csharp
string first = "Hello";
string second = first;           // both reference the same data (until modified)
```

Strings are immutable in C#.

---

## Practice
1. Declare variables of every major type and print them.
2. Try assigning `null` to a normal `int` (should fail) and to an `int?`.
3. Convert a string to an integer safely using `TryParse`.
4. Experiment with `var`.

---

## Next Step
→ [04. Input & Output](04-input-and-output.md)
