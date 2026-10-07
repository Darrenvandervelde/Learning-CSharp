# 12. Collections & Generics (Basics)

## Goal
Use strongly-typed collections and understand why generics matter.

---

## 12.1 Why Generics?

Without generics you would use `ArrayList` (stores `object`) and need casting.  
With generics you get type safety and better performance.

```csharp
List<int> numbers = new List<int>();   // only ints allowed
```

---

## 12.2 Common Generic Collections

```csharp
using System.Collections.Generic;

// List – dynamic array
List<string> names = new List<string> { "Aria", "Kael" };

// Dictionary – key/value pairs
Dictionary<string, int> scores = new Dictionary<string, int>();
scores["Aria"] = 100;
scores["Kael"] = 85;

// HashSet – unique items
HashSet<int> unique = new HashSet<int> { 1, 2, 2, 3 };  // contains 1,2,3
```

---

## 12.3 Iterating

```csharp
foreach (var pair in scores)
{
    Console.WriteLine($"{pair.Key}: {pair.Value}");
}
```

---

## 12.4 Basic LINQ (Introduction)

```csharp
using System.Linq;

var highScores = scores.Where(s => s.Value >= 90);
var namesOnly = scores.Select(s => s.Key);
var first = scores.FirstOrDefault(s => s.Value > 80);
```

LINQ is extremely powerful — you will use it a lot later.

---

## Practice
1. Create a `List<string>` of names and print them.
2. Create a `Dictionary` of player scores and look up a value.
3. Use `Where` to filter a list.
4. Remove duplicates with a `HashSet`.

---

## Next Step
→ [13. File I/O](13-file-io.md)
