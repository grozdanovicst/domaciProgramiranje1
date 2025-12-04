# Домаћи задатак из Техничке документације

## Задатак  
Написати програм који на основу унете дужине странице квадрата `a` израчунава дужину дијагонале `d`.

**Формула:**  

$`d = 𝑎\sqrt{2}`$

### Алгоритамска шема
```mermaid
  graph TD
    A[Унеси број а]--->B
    B[Израчунавање d = a * sqrt(2)]--->C
    C[Испис резултата d]--->D
    D[Kraj]
```

## Решење
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Unesi duzinu stranice kvadrata a: ");
        double a = double.Parse(Console.ReadLine());

        double d = a * Math.Sqrt(2);

        Console.WriteLine("Duzina dijagonale kvadrata je: " + d);
    }
}
```
### Тест примери

Тест пример 1:

```text
Unesi duzinu stranice kvadrata a: 67
Duzina dijagonale kvadrata je: 94.7523086789974
```

Тест пример 2:

```text
Unesi duzinu stranice kvadrata a: 23
Duzina dijagonale kvadrata je: 32.5269119345812
```

### Објекти

| Редни број | Променљива  | Тип променљиве   |
|------------|-------------|------------------|
| 1.         | a           | 'double'         |
| 2.         | d           | 'double'         |
