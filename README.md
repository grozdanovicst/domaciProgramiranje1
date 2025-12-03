# Домаћи задатак из Техничке документације

## Задатак  
Написати програм који на основу унете дужине странице квадрата `a` израчунава дужину дијагонале `d`.

**Формула:**  

$`d = 𝑎\sqrt{2}`$

### Алгоритамска шема
```mermaid
  flowchart TD
    A([Početak])
    B[/Unos vrednosti a/]
    C[Izračunavanje\n d = a * sqrt(2)]
    D[\Ispis rezultata d/]
    E([Kraj])

    A --> B --> C --> D --> E
```

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Unesi dužinu stranice kvadrata a: ");
        double a = double.Parse(Console.ReadLine());

        double d = a * Math.Sqrt(2);

        Console.WriteLine("Dužina dijagonale kvadrata je: " + d);
    }
}
```

### Тест примери

| Тест | Улаз (a) | Излаз (d = a·√2) |
|------|-----------|------------------|
| 1    | 1         | 1.41421356       |
| 2    | 2         | 2.82842712       |
| 3    | 5         | 7.07106781       |
| 4    | 10        | 14.14213562      |
