# Vollständige Dateiliste / Complete File List

## Ressourcenpaket: Größere Hotbar / Resource Pack: Larger Hotbar

Dieses Verzeichnis enthält ein vollständiges Minecraft Bedrock Edition Ressourcenpaket, das die Hotbar größer macht.

This directory contains a complete Minecraft Bedrock Edition resource pack that makes the hotbar larger.

---

## Alle Dateien / All Files

### 1. manifest.json
- **Typ / Type**: JSON Konfigurationsdatei / JSON configuration file
- **Zweck / Purpose**: Definiert Paket-Metadaten, Version und UUIDs / Defines pack metadata, version and UUIDs
- **Erforderlich / Required**: Ja / Yes
- **UUID Header**: 6423d417-3bfa-4f02-9261-a4503fa8049d
- **UUID Module**: 5b355b56-eee8-46f9-808b-3bb398b599d9

### 2. ui/hud_screen.json
- **Typ / Type**: JSON UI-Definitionsdatei / JSON UI definition file
- **Zweck / Purpose**: Überschreibt Hotbar-Elemente mit größeren Größen / Overrides hotbar elements with larger sizes
- **Erforderlich / Required**: Ja / Yes
- **Größenänderungen / Size changes**:
  - Slot-Größe: 20x22 → 30x33 (50% größer / 50% larger)
  - Icon-Größe: 16x16 → 24x24 (50% größer / 50% larger)
  - Auswahlrahmen: 24x24 → 36x36 (50% größer / 50% larger)

### 3. README.md
- **Typ / Type**: Markdown Dokumentation / Markdown documentation
- **Sprache / Language**: Englisch / English
- **Zweck / Purpose**: Installations- und Nutzungsanleitung / Installation and usage guide
- **Erforderlich / Required**: Empfohlen / Recommended

### 4. README_DE.md
- **Typ / Type**: Markdown Dokumentation / Markdown documentation
- **Sprache / Language**: Deutsch / German
- **Zweck / Purpose**: Installations- und Nutzungsanleitung / Installation and usage guide
- **Erforderlich / Required**: Optional

### 5. FOLDER_STRUCTURE.md
- **Typ / Type**: Markdown Dokumentation / Markdown documentation
- **Sprache / Language**: Zweisprachig (DE/EN) / Bilingual (DE/EN)
- **Zweck / Purpose**: Erklärt die Ordnerstruktur und Anpassungen / Explains folder structure and customization
- **Erforderlich / Required**: Optional

### 6. pack_icon_instructions.txt
- **Typ / Type**: Text Dokumentation / Text documentation
- **Zweck / Purpose**: Anweisungen zum Erstellen eines Pack-Icons / Instructions for creating a pack icon
- **Erforderlich / Required**: Optional
- **Hinweis / Note**: Du kannst eine pack_icon.png Datei (256x256) hinzufügen / You can add a pack_icon.png file (256x256)

### 7. FILE_LIST.md
- **Typ / Type**: Markdown Dokumentation / Markdown documentation
- **Zweck / Purpose**: Diese Datei - Übersicht aller Dateien / This file - Overview of all files
- **Erforderlich / Required**: Optional

---

## Minimale Dateien für funktionierendes Paket / Minimum Files for Working Pack

Nur diese Dateien sind technisch erforderlich:
Only these files are technically required:

```
larger_hotbar_pack/
├── manifest.json              ← ERFORDERLICH / REQUIRED
└── ui/
    └── hud_screen.json       ← ERFORDERLICH / REQUIRED
```

Alle anderen Dateien sind Dokumentation.
All other files are documentation.

---

## Installation

### Methode 1: Ordner kopieren / Method 1: Copy Folder

Kopiere den gesamten `larger_hotbar_pack` Ordner nach:
Copy the entire `larger_hotbar_pack` folder to:

**Windows**:
```
%localappdata%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs\larger_hotbar_pack\
```

**Android**:
```
/storage/emulated/0/games/com.mojang/resource_packs/larger_hotbar_pack/
```

**iOS**:
```
Apps/com.mojang.minecraftpe/Documents/games/com.mojang/resource_packs/larger_hotbar_pack/
```

### Methode 2: Als .mcpack (Optional) / Method 2: As .mcpack (Optional)

1. Zippe alle Dateien im `larger_hotbar_pack` Ordner / Zip all files in the `larger_hotbar_pack` folder
2. Benenne die .zip Datei um zu .mcpack / Rename the .zip file to .mcpack
3. Öffne die .mcpack Datei mit Minecraft / Open the .mcpack file with Minecraft

```bash
cd larger_hotbar_pack
zip -r ../larger_hotbar_pack.mcpack *
```

---

## Anpassung / Customization

Um die Größe anzupassen, bearbeite `ui/hud_screen.json`:
To adjust the size, edit `ui/hud_screen.json`:

**Größere Hotbar (z.B. 100% größer) / Larger Hotbar (e.g., 100% larger)**:
- Ändere `[30, 33]` zu `[40, 44]` / Change `[30, 33]` to `[40, 44]`
- Ändere `[24, 24]` zu `[32, 32]` / Change `[24, 24]` to `[32, 32]`
- Ändere `[36, 36]` zu `[48, 48]` / Change `[36, 36]` to `[48, 48]`

**Kleinere Hotbar (z.B. 25% größer) / Smaller Hotbar (e.g., 25% larger)**:
- Ändere `[30, 33]` zu `[25, 27.5]` / Change `[30, 33]` to `[25, 27.5]`
- Ändere `[24, 24]` zu `[20, 20]` / Change `[24, 24]` to `[20, 20]`
- Ändere `[36, 36]` zu `[30, 30]` / Change `[36, 36]` to `[30, 30]`

---

## Technische Informationen / Technical Information

- **Format Version**: 2
- **Minimum Minecraft Version**: 1.21.0
- **Pakettyp / Pack Type**: Resources (UI)
- **Kompatibilität / Compatibility**: Alle Plattformen / All platforms

---

## Zusammenfassung / Summary

✅ **6-7 Dateien total** (+ optional pack_icon.png)  
✅ **2 erforderliche Dateien** (manifest.json, ui/hud_screen.json)  
✅ **4-5 optionale Dokumentationsdateien**  
✅ **Einzigartige UUIDs generiert**  
✅ **Funktionsfähiges Ressourcenpaket**  
✅ **Anpassbar für verschiedene Größen**  

✅ **6-7 files total** (+ optional pack_icon.png)  
✅ **2 required files** (manifest.json, ui/hud_screen.json)  
✅ **4-5 optional documentation files**  
✅ **Unique UUIDs generated**  
✅ **Working resource pack**  
✅ **Customizable for different sizes**
