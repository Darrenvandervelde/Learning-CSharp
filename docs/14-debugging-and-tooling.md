# 14. Debugging & Tooling

## Goal
Become comfortable finding and fixing bugs, and using the .NET ecosystem tools.

---

## 14.1 Using the Debugger

In Visual Studio / VS Code / Rider:

- Set **breakpoints** by clicking left of a line number
- Press F5 (or the play button) to start debugging
- **Step Over** (F10) – execute current line
- **Step Into** (F11) – go into a method
- **Step Out** – finish the current method
- Hover over variables or use the Watch / Locals window

Practice this early — it saves hours later.

---

## 14.2 Common Runtime Exceptions

- `NullReferenceException` → something is null
- `IndexOutOfRangeException` → bad index
- `FormatException` → bad conversion
- `InvalidOperationException` → wrong state

Read the stack trace carefully — it tells you exactly where the problem occurred.

---

## 14.3 NuGet Package Management

```bash
dotnet add package Newtonsoft.Json
dotnet add package Serilog
dotnet list package
dotnet remove package PackageName
```

Or use the NuGet UI in your IDE.

---

## 14.4 Useful Tools

- **dotnet CLI** – create, build, run, test, publish
- **NuGet** – package manager
- **dotnet format** – code style
- **Unit testing** frameworks (xUnit, NUnit, MSTest) – learn later

---

## Practice
1. Place breakpoints and step through a small program.
2. Force a `NullReferenceException` and inspect it in the debugger.
3. Add a NuGet package and use it.
4. Read a full stack trace and locate the source of an error.

---

## Next Step
→ [15. Good Practices for Beginners](15-good-practices.md)
