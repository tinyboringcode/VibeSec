# VIBESEC

> Vigilant Inspector for Bugs and Exploits in Software Engineering Code

![License](https://img.shields.io/badge/license-MIT-blue)
![Status](https://img.shields.io/badge/status-early%20alpha-red)

**VibeSec** to otwartoźródłowe narzędzie do statycznej analizy kodu Python, zaprojektowane z myślą o bezpieczeństwie, dobrych praktykach i vibe codingu.

### 🎯 Dlaczego?

AI pisze kod. Ale nie sprawdza go z ludzką czujnością.  
VibeSec to Twój cichy partner, który tropi błędy, niebezpieczne wzorce i podatne zależności, zanim trafią na produkcję.

---

## 🔧 Funkcje

- 🔍 Analiza plików `.py` pod kątem niebezpiecznych wzorców (np. `eval`, `os.system`)
- 🧠 Wyjaśnienia ryzyk i lepsze alternatywy
- 📦 Sprawdzanie zależności z `requirements.txt` pod kątem znanych podatności (CVE)
- 🧱 Prosta integracja przez CLI lub `import vibesec`

---

## 🚀 Przykład użycia

```python
from vibesec import analyze_file

report = analyze_file("app/main.py")
for issue in report:
    print(issue)
