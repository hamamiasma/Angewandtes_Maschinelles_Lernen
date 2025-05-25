# Jupyter Notebooks - SoSe 2025

## Kursübersicht

- **Software-Stack:** Python, NumPy, SciKit-Learn, Jupyter Notebooks

## Exercise 1 - Themen
- Nearest Neighbour Classifier
- Train- und Test-Accuracy
- Hyperparameter und Hyperparameter-Optimierung
- Cross-Validation und Grid-Search
- Scikit-Learn Verwendung

## Python-Bibliotheken für Data Science
- **NumPy:** Arrays und lineare Algebra
- **Jupyter Notebook:** Browser-basierte Programmierumgebung
- **Matplotlib/Seaborn:** Datenvisualisierung
- **Pandas:** Datenanalyse und -manipulation
- **SciKit-Learn:** Machine Learning

## Setup-Optionen

### 1. Lokale Installation (Empfohlen)
```bash
# 1. Miniconda installieren von: https://docs.conda.io/en/latest/miniconda.html
# 2. Conda-Environment erstellen
conda create -n aml python=3.10

# 3. Environment aktivieren
conda activate aml

# 4. Bibliotheken installieren
conda install numpy pandas matplotlib seaborn

# 5. Jupyter Notebook installieren
conda install -c conda-forge notebook

# 6. Jupyter Notebook starten
jupyter notebook
```

### 2. JupyterHub der HU Berlin
- **URL:** https://jupyterhub.cms.hu-berlin.de/
- **Zugang:** Nur HU-intern (VPN erforderlich bei Remote-Zugriff)
- **Vorteil:** Keine lokale Installation nötig
- **Nachteil:** Keine kollaborative Arbeit möglich

### 3. Google Colab
- **URL:** https://colab.research.google.com/
- **Zugang:** Google-Account erforderlich
- **Vorteile:** Cloud-basiert, kollaborative Arbeit möglich
- **Speicherort:** Google Drive (Ordner "Colab Notebooks")

### 4. PyCharm
- **Kostenlose Version:** Für akademische Nutzung verfügbar
- **Features:** IDE mit Jupyter Notebook-Support und Debugging

## Jupyter Notebook Grundlagen

### Zelltypen
- **Code-Zellen:** Python-Code ausführen
- **Markdown-Zellen:** Dokumentation und Struktur

### Wichtige Shortcuts
- **Ctrl + Enter:** Code ausführen
- **Shift + Enter:** Code ausführen und neue Zelle erstellen
- **Tab:** Autocomplete
- **Shift + Tab:** Funktionssignatur anzeigen

### Markdown-Syntax
```markdown
# Überschrift 1
## Überschrift 2
### Überschrift 3
```

## Debugging-Optionen
1. **Print-Statements:** Einfachste Methode für schnelles Debugging
2. **Stack Trace:** Zeigt Aufrufstapel bei Fehlern
3. **Debug-Modus:** In JupyterHub verfügbar
4. **PyCharm Debugger:** Professionelle IDE-Debugging-Tools

## Python Basics Selbststudium
Falls Sie Python lernen möchten, stehen folgende Notebooks zur Verfügung:
- `ML-SS-2020-Python-1-Types.ipynb` - Datentypen
- `ML-SS-2020-Python-2-Composite-Data.ipynb` - Zusammengesetzte Daten
- `ML-SS-2020-Python-3-Dictionaries-Sets.ipynb` - Dictionaries und Sets
- `ML-SS-2020-Python-4-Controll-Blocks.ipynb` - Kontrollstrukturen

## Wichtige Python-Konzepte

### Datentypen
- **Immutable:** int, float, string, tuple
- **Mutable:** list, dict, set

### Sequence Types
- **Tuple:** `()` - unveränderlich, geordnet
- **List:** `[]` - veränderlich, geordnet
- **String:** `""` - unveränderlich, Zeichenfolge

### Indexing und Slicing
```python
# Indexing (beginnt bei 0)
my_list[0]    # Erstes Element
my_list[-1]   # Letztes Element

# Slicing [start:end]
my_list[1:3]  # Elemente 1 bis 2 (3 nicht eingeschlossen)
```

### Wichtige Operationen
- **Listen:** append(), insert(), extend(), remove(), sort()
- **Dictionaries:** keys(), values(), items()
- **Membership:** `in` Operator
- **Concatenation:** `+` Operator

### Kontrollstrukturen
- **Conditionals:** if/else-Bedingungen
- **Loops:** for-Schleifen über Sequenzen
- **List Comprehensions:** Kompakte Listenerstellung

### Funktionen
```python
def function_name(parameter):
    return result

# Lambda-Funktionen
lambda x: x**2
```

## Nützliche Ressourcen
- **Jupyter Notebooks:** https://jupyter.org
- **Anaconda:** https://www.anaconda.com
- **Google Colab:** https://colab.research.google.com
- **Online Courses:** https://www.deeplearning.ai
- **Bücher:** 
  - http://ciml.info/
  - https://web.stanford.edu/~hastie/ElemStatLearn/

## Tipps für den Kurserfolg
1. Arbeiten Sie regelmäßig an den Assignments
2. Nutzen Sie die automatischen Testfälle
3. Arbeiten Sie effektiv im 3er-Team
