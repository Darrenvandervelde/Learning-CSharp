# 6. Control Flow

## Goal
Control the flow of execution with decisions and loops.

---

## 6.1 if / else if / else

```csharp
int score = 85;

if (score >= 90)
{
    Console.WriteLine("A");
}
else if (score >= 80)
{
    Console.WriteLine("B");
}
else
{
    Console.WriteLine("C or lower");
}
```

---

## 6.2 switch Statement & Switch Expression

Classic switch:

```csharp
int day = 3;

switch (day)
{
    case 1:
        Console.WriteLine("Monday");
        break;
    case 2:
        Console.WriteLine("Tuesday");
        break;
    default:
        Console.WriteLine("Other day");
        break;
}
```

Modern switch expression (C# 8+):

```csharp
string result = day switch
{
    1 => "Monday",
    2 => "Tuesday",
    3 => "Wednesday",
    _ => "Other day"
};
```

---

## 6.3 Loops

### for
```csharp
for (int i = 0; i < 5; i++)
{
    Console.WriteLine(i);
}
```

### foreach
```csharp
int[] numbers = { 10, 20, 30 };
foreach (int n in numbers)
{
    Console.WriteLine(n);
}
```

### while
```csharp
int i = 0;
while (i < 5)
{
    Console.WriteLine(i);
    i++;
}
```

### do-while
```csharp
int number;
do
{
    Console.Write("Enter a positive number: ");
    number = int.Parse(Console.ReadLine());
} while (number <= 0);
```

---

## 6.4 break and continue

```csharp
for (int i = 0; i < 10; i++)
{
    if (i == 3) continue;   // skip this iteration
    if (i == 7) break;      // exit loop
    Console.WriteLine(i);
}
```

---

## Practice
1. Print numbers 1 to 100.
2. Print only even numbers.
3. Create a simple number guessing game.
4. Use a switch expression for menu options.

---

## Next Step
→ [07. Methods](07-methods.md)
