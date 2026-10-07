# 4. Input & Output

## Goal
Learn how to display information and read user input in console applications.

---

## 4.1 Output

```csharp
Console.WriteLine("Hello, World!");   // with newline
Console.Write("No newline");          // without newline

int age = 25;
Console.WriteLine("I am " + age + " years old.");

// String interpolation (preferred)
Console.WriteLine($"I am {age} years old.");
```

---

## 4.2 Input

```csharp
Console.Write("Enter your name: ");
string name = Console.ReadLine();

Console.WriteLine($"Hello, {name}!");
```

`Console.ReadLine()` always returns a `string` (or `null`).

---

## 4.3 Converting Input

```csharp
Console.Write("Enter your age: ");
string input = Console.ReadLine();

if (int.TryParse(input, out int age))
{
    Console.WriteLine($"You are {age} years old.");
}
else
{
    Console.WriteLine("Invalid number.");
}
```

Always prefer `TryParse` over `Parse` or `Convert` when dealing with user input.

---

## 4.4 Reading Multiple Values

```csharp
Console.Write("Enter two numbers: ");
string line = Console.ReadLine();
string[] parts = line.Split(' ');

if (parts.Length == 2 &&
    int.TryParse(parts[0], out int a) &&
    int.TryParse(parts[1], out int b))
{
    Console.WriteLine($"Sum: {a + b}");
}
```

---

## 4.5 Basic Formatting

```csharp
double price = 19.99;
Console.WriteLine($"Price: {price:C}");          // Currency
Console.WriteLine($"Value: {price:F2}");         // 2 decimal places
Console.WriteLine($"Percent: {0.85:P}");         // Percentage
```

---

## Practice
1. Ask for the user’s name and age, then print a greeting.
2. Read two numbers and print their sum, difference, product, and quotient.
3. Safely parse input and handle invalid numbers.
4. Format a decimal number as currency.

---

## Next Step
→ [05. Operators](05-operators.md)
