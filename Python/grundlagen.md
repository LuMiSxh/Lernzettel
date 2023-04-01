# Grundlagen

Innerhalb dieser Datei findest du die Grundlagen, die für das Programmieren mit Python notwendig sind.

---

## Variablen

```py
# Variablen können Werte speichern
x = 5
y = "Hallo"
```

## Datentypen

```py
# Verschiedene Datentypen in Python
x = 5  # Integer
y = 3.14  # Float
z = "Hallo"  # String
a = True  # Boolean
b = [1, 2, 3]  # Liste
c = (4, 5, 6)  # Tuple
d = {"name": "Max", "age": 25}  # Dictionary
```

# Schleifen

```py
# Schleifen werden verwendet, um Code wiederholt auszuführen
for i in range(5):
    print(i)

while True:
    print("Endlos-schleife!")
```

# Funktionen

## Definieren

```py
# Funktionen werden verwendet, um Code zu strukturieren und wiederverwendbar zu machen
def add_numbers(a, b):
    return a + b
```

## Aufrufen

```py
# Funktionen können mit Parametern aufgerufen werden
result = add_numbers(2, 3)
print(result)  # Output: 5
```

# Module und Pakete

## Module importieren

```py
# Module werden verwendet, um zusätzliche Funktionen und Variablen bereitzustellen
import math

result = math.sqrt(16)
print(result)  # Output: 4.0
```

## Pakete importieren

```py
# Pakete sind Sammlungen von Modulen und können ebenfalls importiert werden
from sklearn.linear_model import LinearRegression

model = LinearRegression()
```

# Klassen

## Definition

```py
class MyClass:
    def __init__(self, arg1, arg2):
        self.attr1 = arg1
        self.attr2 = arg2

    def my_method(self):
        print("Hello, World!")
```

* `class` - Schlüsselwort, um eine Klasse zu definieren.
* `MyClass` - Name der Klasse.
* `__init__` - Konstruktor-Methode, um eine Instanz der Klasse zu erstellen. Der Konstruktor wird aufgerufen, wenn ein
  neues Objekt der Klasse erstellt wird.
* `self` - das erste Argument jeder Methodendefinition, das die Instanz selbst darstellt.
* `arg1, arg2` - Parameter, die dem Konstruktor übergeben werden.
* `self.attr1, self.attr2` - Attribute (Variablen) der Klasse.
* `my_method` - Methode (Funktion) der Klasse.

## Objektorientierte Programmierung (OOP)

OOP ist ein Programmierparadigma, bei dem alles als Objekt betrachtet wird, das eine Instanz einer Klasse ist. Eine
Instanz ist ein spezielles Exemplar einer Klasse und hat Zugriff auf die Attribute und Methoden der Klasse.

## Erstellen einer Objektinstanz

```py
my_object = MyClass("Value 1", "Value 2")
```

# Verwendung von Attributen

```py
print(my_object.attr1)
```

## Verwendung von Methoden / Funktionen

```py
my_object.my_method()
```

## Vererbung

```py
class MyChildClass(MyClass):
    def my_child_method(self):
        print("I am a child method!")
```

* `MyChildClass` - Name der abgeleiteten Klasse.
* `MyClass` - Name der Basisklasse.
* `my_child_method` - Methode der abgeleiteten Klasse.

## Polymorphismus

Polymorphismus ist ein Konzept in der OOP, bei dem Objekte unterschiedliche Formen annehmen können. Das bedeutet, dass
eine Methode in verschiedenen Klassen unterschiedliche Dinge tun kann.

```py
class MyOtherClass:
    def my_method(self):
        print("Hello, from another class!")


my_objects = [MyClass("Value 1", "Value 2"), MyOtherClass()]

for obj in my_objects:
    obj.my_method()
```

* `MyOtherClass` - eine andere Klasse.
* `my_objects` - eine Liste von Objekten unterschiedlicher Klassen.
* `for` - eine Schleife, die jedes Objekt in der Liste durchläuft.
* `obj.my_method()` - ruft die `my_method()` Methode jedes Objekts auf, die unterschiedliche Dinge tun wird, je nachdem, welcher Klasse das Objekt angehört
