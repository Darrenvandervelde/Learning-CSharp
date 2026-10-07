# 10. Inheritance & Polymorphism (Introduction)

## Goal
Learn how to reuse and extend code through inheritance and polymorphism.

---

## 10.1 Inheritance

```csharp
class Animal
{
    public string Name { get; set; }

    public virtual void Speak()
    {
        Console.WriteLine("Some sound");
    }
}

class Dog : Animal
{
    public override void Speak()
    {
        Console.WriteLine("Woof!");
    }
}

Dog dog = new Dog { Name = "Rex" };
dog.Speak();   // Woof!
```

---

## 10.2 base Keyword

```csharp
class Dog : Animal
{
    public Dog(string name)
    {
        Name = name;
    }

    public override void Speak()
    {
        base.Speak();          // call parent version
        Console.WriteLine("Woof!");
    }
}
```

---

## 10.3 Abstract Classes

```csharp
abstract class Shape
{
    public abstract double Area();
}

class Circle : Shape
{
    public double Radius { get; set; }

    public override double Area() => Math.PI * Radius * Radius;
}
```

You cannot create an instance of an abstract class.

---

## 10.4 Interfaces (Introduction)

```csharp
interface IDamageable
{
    void TakeDamage(int amount);
}

class Player : IDamageable
{
    public int Health { get; set; }

    public void TakeDamage(int amount)
    {
        Health -= amount;
    }
}
```

A class can implement multiple interfaces.

---

## 10.5 Polymorphism in Practice

```csharp
Animal[] animals = { new Dog(), new Animal() };

foreach (Animal a in animals)
{
    a.Speak();   // calls the correct version
}
```

---

## Practice
1. Create a base `Enemy` class and two derived classes (`Goblin`, `Dragon`).
2. Override a method in the derived classes.
3. Create an abstract class with an abstract method.
4. Define a simple interface and implement it.

---

## Next Step
→ [11. Exception Handling](11-exception-handling.md)
