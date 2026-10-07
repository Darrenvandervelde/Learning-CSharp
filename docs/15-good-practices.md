# 15. Good Practices for Beginners

## Goal
Build solid habits from the beginning.

---

## 15.1 Follow C# Naming Conventions

- PascalCase for classes, methods, properties
- camelCase for local variables and parameters
- Meaningful names over short names

---

## 15.2 Prefer Properties over Public Fields

```csharp
// Prefer
public int Health { get; set; }

// Avoid
public int health;
```

---

## 15.3 Keep Methods Small and Focused

A method should do one thing and do it well.

---

## 15.4 Handle Null Safely

Use `?.`, `??`, and `is not null` checks.

---

## 15.5 Write Readable Code First

Optimize only when you have measured a real problem.

---

## 15.6 Use the Type System

Let the compiler help you. Prefer strong types over `object` or lots of casting.

---

## 15.7 Practice Daily

- Solve small problems
- Rebuild old programs with better structure
- Read clean code examples

---

## Final Advice

C# is a very productive language. Master the fundamentals (especially OOP, collections, and exception handling) and you will be able to build real applications quickly.

Happy coding!
