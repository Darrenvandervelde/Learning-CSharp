# 11. Exception Handling

## Goal
Handle runtime errors gracefully instead of crashing.

---

## 11.1 try / catch / finally

```csharp
try
{
    Console.Write("Enter a number: ");
    int number = int.Parse(Console.ReadLine());
    Console.WriteLine(10 / number);
}
catch (FormatException)
{
    Console.WriteLine("That was not a valid number.");
}
catch (DivideByZeroException)
{
    Console.WriteLine("Cannot divide by zero.");
}
catch (Exception ex)   // general catch (use sparingly)
{
    Console.WriteLine($"Unexpected error: {ex.Message}");
}
finally
{
    Console.WriteLine("This always runs.");
}
```

---

## 11.2 Throwing Exceptions

```csharp
void SetAge(int age)
{
    if (age < 0)
        throw new ArgumentException("Age cannot be negative.");

    // ...
}
```

---

## 11.3 Common Exception Types

| Exception                  | Typical Cause                     |
|----------------------------|-----------------------------------|
| `FormatException`          | Invalid string conversion         |
| `DivideByZeroException`    | Division by zero                  |
| `NullReferenceException`   | Using a null object               |
| `IndexOutOfRangeException` | Bad array/list index              |
| `ArgumentException`        | Invalid argument passed           |
| `FileNotFoundException`    | Missing file                      |

---

## 11.4 Best Practices

- Catch specific exceptions when possible
- Don’t swallow exceptions silently
- Use `finally` (or `using`) for cleanup
- Throw meaningful exceptions with clear messages

---

## Practice
1. Write a program that safely reads an integer from the user.
2. Create a method that throws an exception for invalid input.
3. Catch multiple exception types separately.
4. Use a `finally` block to print a message.

---

## Next Step
→ [12. Collections & Generics](12-collections-and-generics.md)
