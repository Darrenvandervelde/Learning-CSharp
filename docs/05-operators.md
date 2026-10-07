# 5. Operators

## Goal
Master the operators used for calculations, comparisons, and logic.

---

## 5.1 Arithmetic Operators

```csharp
int a = 10, b = 3;

Console.WriteLine(a + b);   // 13
Console.WriteLine(a - b);   // 7
Console.WriteLine(a * b);   // 30
Console.WriteLine(a / b);   // 3  (integer division)
Console.WriteLine(a % b);   // 1  (remainder)

double result = 10.0 / 3.0; // 3.333...
```

---

## 5.2 Comparison Operators

```csharp
int x = 5, y = 10;

x == y   // false
x != y   // true
x < y    // true
x > y    // false
x <= y   // true
x >= y   // false
```

---

## 5.3 Logical Operators

```csharp
bool isAdult = true;
bool hasLicense = false;

isAdult && hasLicense   // false (AND)
isAdult || hasLicense   // true  (OR)
!isAdult                // false (NOT)
```

---

## 5.4 Assignment & Compound Assignment

```csharp
int x = 10;
x += 5;   // 15
x -= 3;   // 12
x *= 2;   // 24
x /= 4;   // 6
x %= 4;   // 2
```

---

## 5.5 Increment & Decrement

```csharp
int i = 5;
++i;      // pre-increment
i++;      // post-increment
--i;
i--;
```

---

## 5.6 Null-related Operators (Very Useful)

```csharp
string name = null;

// Null-coalescing
string display = name ?? "Unknown";

// Null-conditional
int? length = name?.Length;

// Null-coalescing assignment
name ??= "Default";
```

---

## 5.7 Ternary Operator

```csharp
int age = 20;
string status = age >= 18 ? "Adult" : "Minor";
```

---

## Practice
1. Calculate the average of three numbers.
2. Check if a number is even or odd.
3. Use `&&` and `||` in conditions.
4. Practice the null-coalescing operator.

---

## Next Step
→ [06. Control Flow](06-control-flow.md)
