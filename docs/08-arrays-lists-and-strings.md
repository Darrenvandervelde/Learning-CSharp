# 8. Arrays, Lists & Strings

## Goal
Work with collections of data and text effectively.

---

## 8.1 Arrays

```csharp
int[] scores = new int[5];
int[] numbers = { 10, 20, 30, 40, 50 };

Console.WriteLine(numbers[0]);     // 10
numbers[1] = 25;

foreach (int n in numbers)
    Console.WriteLine(n);
```

Arrays have a fixed size once created.

---

## 8.2 Multidimensional Arrays

```csharp
int[,] matrix = new int[2, 3]
{
    { 1, 2, 3 },
    { 4, 5, 6 }
};

Console.WriteLine(matrix[1, 2]);   // 6
```

---

## 8.3 List<T> (Preferred for most cases)

```csharp
using System.Collections.Generic;

List<int> scores = new List<int> { 90, 85, 78 };
scores.Add(92);
scores.Remove(85);

Console.WriteLine(scores.Count);
Console.WriteLine(scores[0]);

foreach (int score in scores)
    Console.WriteLine(score);
```

`List<T>` grows dynamically and is much more convenient than arrays for most scenarios.

---

## 8.4 Strings

```csharp
string name = "Darren";
string greeting = $"Hello, {name}!";

Console.WriteLine(name.Length);
Console.WriteLine(name.ToUpper());
Console.WriteLine(name.Contains("arr"));
Console.WriteLine(name.Substring(0, 3));   // "Dar"
```

Strings are immutable. Every modification creates a new string.

For heavy string building, use `StringBuilder`:

```csharp
using System.Text;

var sb = new StringBuilder();
sb.Append("Hello");
sb.Append(" World");
string result = sb.ToString();
```

---

## Practice
1. Create an array and a List of integers and print them.
2. Find the maximum value in a List.
3. Reverse a string.
4. Count occurrences of a character in a string.

---

## Next Step
→ [09. Object-Oriented Programming Basics](09-oop-basics.md)
