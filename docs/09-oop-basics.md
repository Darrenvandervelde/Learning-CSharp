# 9. Object-Oriented Programming (Basics)

## Goal
Start organizing code using classes and objects.

---

## 9.1 Classes and Objects

```csharp
class Player
{
    public string Name;
    public int Health;

    public void TakeDamage(int amount)
    {
        Health -= amount;
        if (Health < 0) Health = 0;
    }
}

Player hero = new Player();
hero.Name = "Aria";
hero.Health = 100;
hero.TakeDamage(25);
```

---

## 9.2 Properties (Preferred over public fields)

```csharp
class Player
{
    public string Name { get; set; }           // auto-property
    public int Health { get; private set; }    // read-only from outside

    public void TakeDamage(int amount)
    {
        Health -= amount;
        if (Health < 0) Health = 0;
    }
}
```

---

## 9.3 Constructors

```csharp
class Player
{
    public string Name { get; set; }
    public int Health { get; set; }

    public Player(string name, int health)
    {
        Name = name;
        Health = health;
    }
}

Player hero = new Player("Aria", 100);
```

---

## 9.4 Access Modifiers

| Modifier     | Accessibility                          |
|--------------|----------------------------------------|
| `public`     | Everywhere                             |
| `private`    | Only inside the class                  |
| `protected`  | Inside the class + derived classes     |
| `internal`   | Inside the same assembly               |

---

## 9.5 Static Members

```csharp
class Game
{
    public static int PlayerCount = 0;

    public Game()
    {
        PlayerCount++;
    }
}
```

---

## Practice
1. Create a `Rectangle` class with Width, Height, and an Area property.
2. Add a constructor.
3. Make fields private and expose them via properties.
4. Create multiple instances and call methods.

---

## Next Step
→ [10. Inheritance & Polymorphism](10-inheritance-and-polymorphism.md)
