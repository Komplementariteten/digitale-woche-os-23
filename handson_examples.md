<style>
    .qr_code {
        position: relative;
        float: right;
        width: 20%;
        margin-right: 10%
    }
</style>

# Module und Pakete
Auf existierende Funktionalitäten zugreifen über Pakete

<br/>
- Eine einzelne Python Datei heißt Modul
<br/>
<br/>
- Mehrere Module können zusammen ein Paket bilden
<br/>
<br/>
- Pakete können auf <em>PyPI</em> (Package Index) hochgeladen werden
<br/>
<br/>
- Über den package installer <em>pip</em> können Pakete von PyPI installiert werden
<br/>
<br/>

```console
pip install 'package_name'
```

---

# Pakete nutzen
<br/>
Installierte Pakete einbinden über <em>import</em> statetement
<br/>
```py
    import os   # Funktionen zur Interaktion mit Betriebssystem
    
    # Aktuelles Arbeitsverzeichnis ermitteln
    cwd = os.getcwd()
    print("Wir sind im Verzeichnis: " + cwd)
```
<br/>
Ausgabe:
```console
    Wir sind im Verzeichnis: C:\digitale-woche-os
```

---


# Pakete nutzen
<br/>
Vielgenutzte Pakete mit Alias importieren
<br/>
```py
    import numpy as np   # Funktionen für Datenverarbeitung
    
    summed_values = np.sum([20, 22])
    print("Die Antwort ist " + str(summed_values))
```
<br/>
Ausgabe:
```console
    Die Antwort ist 42
```

---

# Programmierbeispiele
Pygame Bibliothek bietet Einstieg in Spieleprogrammierung

<img src="/qr-code_pygame.png" alt = "QR pygame" class = "qr_code"/>
<br/>
<br/>
<br/>
Code mit Web-Interpreter öffnen: <a href = "https://trinket.io/pygame/b118fa0281"> https://trinket.io/pygame/b118fa0281 </a>

<br/>
<br/>
Code verfügbar auf <br/>
 <a href = "https://github.com/afey89/python_workshop_2023/tree/main/src/pygame_example"> https://github.com/afey89/python_workshop_2023/tree/main/src/pygame_example </a>

---

# Beispiel Datenanalyse
Datenanalyse mit Numpy und Matplotlib

<img src="/qr-code_data_analysis.png" alt = "QR data analysis" class = "qr_code"/>
<br/>
<br/>
<br/>
Code mit Web-Interpreter öffnen: <a href = "https://trinket.io/python3/aa6ca645eb"> https://trinket.io/python3/aa6ca645eb </a>

<br/>
<br/>
Code verfügbar auf: <br/>
 <a href = "https://github.com/afey89/python_workshop_2023/tree/main/src/pygame_example"> https://github.com/afey89/python_workshop_2023/tree/main/src/pygame_example </a>