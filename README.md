# LaTeX-Vorlage für wissenschaftliche Arbeiten (IU-konform)

![IU-Logo](https://raw.githubusercontent.com/timootten/IU-Latex/refs/heads/main/assets/iu-logo.png)  
_(Hinweis: Dies ist keine offizielle Vorlage der IU Internationalen Hochschule.)_

---

## 📜 Über dieses Projekt

Diese LaTeX-Vorlage wurde von **Timo Otten** (dualer Student an der IU) erstellt, um Kommiliton:innen die Formatierung wissenschaftlicher Arbeiten nach IU-Richtlinien zu erleichtern.  
**Wichtig:**

- 🚨 **Keine Gewähr** – Ich übernehme **keine Haftung** für Fehler in der Vorlage oder daraus resultierende Probleme.
- 📄 **Keine offizielle IU-Vorlage** – Nutzung auf eigene Verantwortung. Immer die aktuellen Richtlinien der IU prüfen!

---

## ⚙️ Installation & Einrichtung für Windows 10/11 mit MikTeX (Empfohlene Software, alternativen möglich)

### 1. Notwendige Software installieren

- **MikTeX** (LaTeX-Distribution):  
  📥 [Download MikTeX](https://miktex.org/)  
  _Wählen Sie während der Installation "Install missing packages on the fly"_

- **Strawberry Perl** (Für Biber/BibTeX):  
  📥 [Download Strawberry Perl](https://strawberryperl.com/)

- **VS Code** (Texteditor):  
  📥 [Download VS Code](https://code.visualstudio.com/)

### 2. VS Code Extensions hinzufügen

- Öffnen Sie VS Code und installieren Sie:
  - 🔍 **LaTeX Workshop** (von James Yu)
  - 🔍 **LaTeX** (von Mathematic Inc)

### 3. Einstellungen für LaTeX Workshop

Fügen Sie in `settings.json` (VS Code) folgende Konfiguration hinzu:

```json
"latex-workshop.latex.tools": [
  {
    "name": "latexmk",
    "command": "latexmk",
    "args": [
      "-xelatex",
      "-synctex=1",
      "-interaction=nonstopmode",
      "-file-line-error",
      "%DOC%"
    ]
  }
]
```
