# Was ist Python?

<br/>
1. Einfach und leserlich
<br/>
<br/>
<br/>
2. Vielseitig einsetzbar
<br/>
<br/>
<br/>
3. Interpretiert und objektorientiert
<br/>
<br/>
<br/>
4. Umfangreiche Standardbibliothek
<br/>
<br/>
<br/>
5. Starke Entwicklergemeinschaft

<PageNr/>

<!--
1. **Einfach und leserlich:** Python ist eine Programmiersprache mit einer leicht verständlichen Syntax, die als "eine Sprache, die man lesen kann" bezeichnet wird.

2. **Vielseitig einsetzbar:** Python kann in verschiedenen Anwendungsbereichen verwendet werden, darunter Webentwicklung, Datenanalyse und künstliche Intelligenz.

3. **Interpretiert und objektorientiert:** Python-Code wird interpretiert und nicht kompiliert. Die Sprache unterstützt die objektorientierte Programmierung.

4. **Umfangreiche Standardbibliothek:** Python bietet eine breite Palette von Modulen und Funktionen in seiner Standardbibliothek, was die Entwicklung beschleunigt.

5. **Starke Entwicklergemeinschaft:** Python hat eine aktive Entwicklergemeinschaft und eine Fülle von Open-Source-Ressourcen.
-->

---
showInToc: false
---

# Entwicklungsumgebung aufsetzen

- Python 3 installieren
  - Windows / Mac OS. [https://www.python.org/downloads/](https://www.python.org/downloads/)
  - Linux (Ubuntu)

    ```bash
    sudo apt-get install python3
    ```

  - Linux (Archlinux)

    ```bash
    sudo pacman -S python3
    ```

  - Linux (build from source)

    ```bash
    ./configure
    make
    make install
    ```

---
hideInToc: true
---

# Visual Studio Code

  <img src="https://upload.wikimedia.org/wikipedia/commons/4/42/VS_Code_1.36.0-insider.png" alt="VS Code" style="height: 300px;"/>

  - Windows / Mac OS: [https://code.visualstudio.com](https://code.visualstudio.com/)
  - Linux See: [https://code.visualstudio.com/docs/setup/linux](https://code.visualstudio.com/docs/setup/linux)

<PageNr/>

---
hideInToc: true
---

# Jupyter Notebooks

<img src="Jupyter.png" style="height: 300px">

[Try Jupyter Online](https://jupyter.org/try-jupyter/lab/)

<PageNr/>

---
transition: fade
---

# Python Grundlagen

- Verschiedene Datentypen:

  ```py
  a = 1 # int

  c = 3.14 # float

  b = True # bool

  d = "Hello" # str

  e = [1, 2, 3] # list

  f = ("Hello", "World") # tuple

  g = { "Name": "Steve", "Alter": "19", "Addresse": "Musterstraße 123" } # dict
  ```

<PageNr/>

---
hideInToc: true
transition: fade
---

# Python Grundlagen

- Ausgabe
  <v-click>

  ```py
  print("Hello, World!")
  # => Hello, World!
  ```

  <br/>
  </v-click>

  <v-click>

  ```py
  a = 34
  print("Der Wert von 'a' ist:", a)
  # => Der Wert von 'a' ist: 34
  ```

  <br/>
  </v-click>

  <v-click>

  ```py
  name = "James"
  print (f"Der Name ist {name}")
  # => Der Name ist James
  ```
  </v-click>
<PageNr/>
---
hideInToc: true
transition: fade
---

# Python Grundlagen

- Operatoren
  <v-click>
  
  ```py
  a + b # Addition
  a - b # Subtraktion

  a * b # Multiplikation
  a / b -> float  | a // b -> int # Division
  a % b # Rest

  a ** b # Exponent
  ```

  <br/>
  </v-click>

  <v-click>

  ```py
  a or b # Oder
  a and b # Und
  not a # Nicht

  a > b # Größer
  a >= b # Größer oder Gleich
  a < b # Kleiner
  a <= b # Kleiner oder Gleich
  a == b # Gleich
  a != b # Ungleich
  ```
  </v-click>

<PageNr/>

---
hideInToc: true
transition: fade
---

# Python Grundlagen

- Zuweisungen

  <v-click>

  ```py
  a = 3
  b = 2

  c = a + b;
  print(c)
  # => 5
  ```

  </v-click>

  <br/>

  <v-click>

  ```py
  a = 7
  b = 3

  a -= b;
  # a = a - b

  print(a)
  # => 4
  ```

  </v-click>

<PageNr/>

---
hideInToc: true
transition: fade
---

# Python Grundlagen

- Kontrollfluss
  <v-click>

  - Bedingte Anweisungen:

  ```py
  alter = 5

  if alter >= 18:
    print("Erwachsen")
  elif (alter >= 14):
    print("Jugendlicher")
  else:
    print("Kind")
  # => Kind
  ```

  </v-click>

  <v-click>

  - Auswahl Operator

  ```py
  alter = 19
  status = "Erwachsen" if alter >= 18 else "Kind"
  print("Erwachsen:", erwachsen)
  # => Status: Erwachsen
  ```

  </v-click>
<PageNr/>
---
hideInToc: true
transition: fade
---

# Python Grundlagen

- Kontrollfluss

  <v-click>

  - 'While'-Schleife:

  ```py
  zaehler = 10
  while zaehler > 0:
    print(zaehler, end=', ')
    zaehler -= 1
  # => 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 
  ```

  </v-click>

  <v-click>

  - 'For'- Schleife:

  ```py
  namen = ["Susanne", "Elisa", "Bert", "Jan"]
  for name in namen:
    print(name, end =', ')
  # => Susanne, Elisa, Bert, Jan, 
  ```

  </v-click>

  <v-click>

  - List Comprehensions:

  ```py
  zahlen = range(1, 6)
  quadratzahlen = [x**2 for x in zahlen]
  print(quadratzahlen)
  # => [1, 4, 9, 16, 25]
  ```
  
  </v-click>

<PageNr/>

---
hideInToc: true
transition: fade
---

# Python Grundlagen

- Kontrollfluss
  - Schleifensteuerung:
    <v-click>

    - break:

    ```py
    zahl = 8
    isPrime = True
    for i in range(2, zahl // 2):
      if zahl % i == 0:
        isPrime = False;
        break
    print("Ist", zahl, "eine Pimzahl:", isPrime)
    # => Ist 8 eine Pimzahl: False
    ```

    </v-click>

    <v-click>

    - continue:

    ```py
    zahlen = [3, 45, 16, 2, 5, 9, 10]
    for zahl in zahlen:
      if zahl % 2 == 0:
        continue
      print(zahl, end=', ')
    # => 3, 45, 5, 9, 
    ```

    </v-click>

<PageNr/>

---
hideInToc: true
transition: fade
---

# Python Grundlagen

- Kontrollfluss
  - Funktionen:

  <v-click>

  ```py
  def add(a, b):
    sum = a + b
    return sum

  print(add(12, 45))
  # => 57
  ```
  
  <br/>

  </v-click>

  <v-click>

  ```py
  def fibonacci(n):
    if n <= 2:
      return 1
    return fibonacci(n-1) + fibonacci(n-2)

  print(fibonacci(4))
  # => 4
  ```

  </v-click>

<PageNr/>
---
hideInToc: true
transition: slide-left
clicks: 1
---


# Python Grundlagen

<style>
  .slidev-vclick-hidden {
    height: 0;
  }
</style>

- Klassen:

<div v-click-hide="1">

```py
class Person:
  def __init__(self, first_name, last_name, age):
    self.first_name = first_name
    self.last_name = last_name
    self.age = age

john = Person("John", "Doe", 37)
print(f"Die Person heißt {john.first_name} {john.last_name} und ist {john.age} Jahre alt")
# => Die Person heißt John Doe und ist 37 Jahre alt

```

</div>

<div v-click="1">

```py
class Person:
  def __init__(self, first_name, last_name, age):
    self.first_name = first_name
    self.last_name = last_name
    self.age = age

  def geburtstag(self):
    self.age += 1

  def __str__(self):
    return f"{self.first_name} {self.last_name}, {self.age} Jahre alt"

john = Person("John", "Doe", 37)

print(john.__str__())
# => John ist 37 Jahre alt

john.geburtstag()

print(john.__str__())
# => John ist 38 Jahre alt
```

</div>

<PageNr/>
---
transition: slide-up
---

<style>
  .code-example {
    border-bottom-width: 0 !important;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    font-size: 60px;
    display: flex;
    flex-direction: row;
  }

  .code-example:hover .code-left {
    animation-name: left;
    animation-duration: 500ms;
  }

  .code-example:hover .code-center {
    animation-name: center;
    animation-duration: 500ms;
  }

  .code-example:hover .code-right {
    animation-name: right;
    animation-duration: 500ms;
  }

  @keyframes left {
    0% {transform: translateX(0)}
    75% {transform: translateX(-20px)}
    100% {transform: translateX(0)}
  }

  @keyframes right {
    0% {transform: translateX(0)}
    75% {transform: translateX(20px)}
    100% {transform: translateX(0)}
  }

  @keyframes center {
    0% {transform: scale(1)}
    75% {transform: scale(1.5)}
    100% {transform: scale(1)}
  }

</style>

# Programmierbeispiel

<a class="code-example" href="https://jupyter.org/try-jupyter/lab/" target="_blank">
  <p class="code-left" >&#60;</p>
  <p class="code-center" >/</p>
  <p class="code-right" >&#62;</p>
  <br/>
</a>

<PageNr/>
