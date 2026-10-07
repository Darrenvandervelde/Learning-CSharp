# 13. File I/O (Basics)

## Goal
Read from and write to files, and get a first look at JSON.

---

## 13.1 Writing Text

```csharp
using System.IO;

File.WriteAllText("message.txt", "Hello, File!");

// Or append
File.AppendAllText("message.txt", "\nSecond line");
```

---

## 13.2 Reading Text

```csharp
string content = File.ReadAllText("message.txt");
Console.WriteLine(content);

string[] lines = File.ReadAllLines("message.txt");
foreach (string line in lines)
    Console.WriteLine(line);
```

---

## 13.3 Working with Paths

```csharp
string path = Path.Combine("data", "save.json");
string full = Path.GetFullPath(path);
```

---

## 13.4 Simple JSON (System.Text.Json)

```csharp
using System.Text.Json;

var player = new { Name = "Aria", Health = 100 };

string json = JsonSerializer.Serialize(player);
File.WriteAllText("player.json", json);

string loaded = File.ReadAllText("player.json");
var restored = JsonSerializer.Deserialize<Dictionary<string, object>>(loaded);
```

For real projects you will define proper classes for serialization.

---

## Practice
1. Write a few lines to a text file and read them back.
2. Create a simple save file using JSON.
3. Check if a file exists before reading it.
4. Use `Path.Combine` to build safe paths.

---

## Next Step
→ [14. Debugging & Tooling](14-debugging-and-tooling.md)
