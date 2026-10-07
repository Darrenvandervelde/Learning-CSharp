# 1. Setup & First Program

## Goal
Get a working C# / .NET development environment and run your first program.

---

## 1.1 Install the .NET SDK

Download and install the latest **LTS** version from the official site:  
[https://dotnet.microsoft.com/download](https://dotnet.microsoft.com/download)

After installation, verify:

```bash
dotnet --version
```

---

## 1.2 Choose an IDE / Editor

| Tool                  | Best For                        | Notes                              |
|-----------------------|---------------------------------|------------------------------------|
| Visual Studio         | Full IDE experience (Windows)   | Excellent debugger & templates     |
| VS Code + C# Dev Kit  | Lightweight & cross-platform    | Free and very popular              |
| JetBrains Rider       | Professional cross-platform     | Paid, outstanding experience       |

---

## 1.3 Create Your First Console App

```bash
dotnet new console -n HelloWorld
cd HelloWorld
dotnet run
```

This creates a simple project and runs it.

---

## 1.4 Understanding the Project Structure

A basic console project looks like this:

```
HelloWorld/
├── HelloWorld.csproj      # Project file (XML)
├── Program.cs             # Entry point
└── obj/ and bin/          # Build outputs (auto-generated)
```

---

## 1.5 Your First Program

Open `Program.cs`:

```csharp
Console.WriteLine("Hello, C#!");
```

With top-level statements (modern C#), you don’t even need a `Main` method for simple programs.

Classic style (still valid):

```csharp
namespace HelloWorld;

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Hello, C#!");
    }
}
```

---

## 1.6 Useful `dotnet` CLI Commands

```bash
dotnet new console          # Create new console app
dotnet build                # Compile the project
dotnet run                  # Build + run
dotnet add package Newtonsoft.Json   # Add a NuGet package
dotnet restore              # Restore packages
```

---

## Practice
1. Change the message and run again.
2. Create a second project and run it.
3. Intentionally make a syntax error and read the error message.

---

## Next Step
→ [02. Basic Syntax & Structure](02-basic-syntax-and-structure.md)
