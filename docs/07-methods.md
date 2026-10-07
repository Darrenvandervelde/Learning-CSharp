# 7. Methods (Functions)

## Goal
Organize code into reusable methods.

---

## 7.1 Basic Method

```csharp
void Greet()
{
    Console.WriteLine("Hello!");
}

Greet();   // call
```

---

## 7.2 Parameters and Return Values

```csharp
int Add(int a, int b)
{
    return a + b;
}

int result = Add(5, 3);   // 8
```

---

## 7.3 Expression-bodied Members

```csharp
int Multiply(int a, int b) => a * b;
```

---

## 7.4 Optional and Named Parameters

```csharp
void PrintMessage(string message = "Hello", int times = 1)
{
    for (int i = 0; i < times; i++)
        Console.WriteLine(message);
}

PrintMessage();                        // uses defaults
PrintMessage("Hi", 3);
PrintMessage(times: 2, message: "Hey"); // named arguments
```

---

## 7.5 ref, out, and in

```csharp
void Double(ref int number)
{
    number *= 2;
}

int x = 10;
Double(ref x);   // x is now 20

bool TryParseAge(string input, out int age)
{
    return int.TryParse(input, out age);
}
```

---

## 7.6 Method Overloading

```csharp
int Add(int a, int b) => a + b;
double Add(double a, double b) => a + b;
```

---

## 7.7 Local Functions

```csharp
void Process()
{
    int helper(int n) => n * 2;   // local function
    Console.WriteLine(helper(5));
}
```

---

## Practice
1. Write a method that returns the maximum of two numbers.
2. Write a method with optional parameters.
3. Create overloaded methods for different types.
4. Use `out` to return multiple values safely.

---

## Next Step
→ [08. Arrays, Lists & Strings](08-arrays-lists-and-strings.md)
