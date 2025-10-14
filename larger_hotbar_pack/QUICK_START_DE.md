# Schnellstart-Anleitung / Quick Start Guide

## 🎮 Größere Hotbar für Minecraft Bedrock Edition

### Was ist das?
Ein Ressourcenpaket, das deine Hotbar in Minecraft Bedrock Edition um 50% vergrößert.

### Was du bekommst:
- ✅ Größere Hotbar-Slots (20x22 → 30x33 Pixel)
- ✅ Größere Item-Icons (16x16 → 24x24 Pixel)  
- ✅ Bessere Sichtbarkeit
- ✅ Anpassbare Größe
- ✅ Einzigartige UUIDs (keine Konflikte)
- ✅ Kompatibel mit allen Plattformen

---

## 🚀 Installation in 3 Schritten

### Schritt 1: Ordner finden
Finde deinen Minecraft Ressourcenpakete-Ordner:

**Windows**:
1. Drücke `Windows + R`
2. Gib ein: `%localappdata%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs\`
3. Drücke Enter

**Android**:
1. Öffne Dateimanager
2. Navigiere zu: `/storage/emulated/0/games/com.mojang/resource_packs/`

**iOS**:
1. Öffne Dateien-App
2. Navigiere zu: `Apps/com.mojang.minecraftpe/Documents/games/com.mojang/resource_packs/`

### Schritt 2: Ordner kopieren
Kopiere den **gesamten** `larger_hotbar_pack` Ordner in den Ressourcenpakete-Ordner.

### Schritt 3: In Minecraft aktivieren
1. Öffne Minecraft Bedrock Edition
2. Gehe zu **Einstellungen**
3. Wähle **Globale Ressourcen**
4. Finde "Larger Hotbar Resource Pack"
5. Klicke auf **+** um es zu aktivieren
6. Klicke **Anwenden**

**Fertig! 🎉**

---

## 📁 Was ist in diesem Ordner?

```
larger_hotbar_pack/
├── manifest.json                 ← Paket-Konfiguration (WICHTIG!)
├── ui/
│   └── hud_screen.json          ← Hotbar-Größen (WICHTIG!)
├── README.md                     ← Englische Anleitung
├── README_DE.md                  ← Deutsche Anleitung
├── FOLDER_STRUCTURE.md           ← Ordner-Erklärung
├── FILE_LIST.md                  ← Alle Dateien erklärt
├── QUICK_START_DE.md            ← Diese Datei
└── pack_icon_instructions.txt    ← Icon-Anweisungen
```

**Nur 2 Dateien sind wirklich notwendig:**
- `manifest.json` 
- `ui/hud_screen.json`

Alle anderen Dateien sind Dokumentation.

---

## ⚙️ Größe anpassen

Möchtest du die Hotbar noch größer oder kleiner machen?

### Datei öffnen
Öffne `ui/hud_screen.json` in einem Texteditor (z.B. Notepad, VS Code)

### Werte ändern
Suche und ersetze diese Werte:

| Was                      | Aktuell     | Beispiel 100% größer | Beispiel 25% größer |
|-------------------------|-------------|---------------------|---------------------|
| Slot-Größe              | `[30, 33]`  | `[40, 44]`          | `[25, 27.5]`       |
| Icon-Größe              | `[24, 24]`  | `[32, 32]`          | `[20, 20]`         |
| Auswahlrahmen           | `[36, 36]`  | `[48, 48]`          | `[30, 30]`         |
| Panel-Höhe              | `33`        | `44`                | `27.5`             |

### Speichern und testen
1. Speichere die Datei
2. Starte Minecraft neu
3. Teste die neue Größe

---

## 🔧 Fehlerbehebung

### ❌ Hotbar wird nicht größer
**Lösungen:**
- [ ] Überprüfe ob das Paket in "Globale Ressourcen" aktiviert ist
- [ ] Starte Minecraft neu
- [ ] Stelle sicher, dass der Ordner korrekt kopiert wurde
- [ ] Überprüfe ob kein anderes Paket die Hotbar überschreibt

### ❌ Minecraft stürzt ab
**Lösungen:**
- [ ] Überprüfe ob die JSON-Dateien korrekt sind
- [ ] Deaktiviere andere Ressourcenpakete
- [ ] Aktualisiere Minecraft auf Version 1.21.0 oder neuer

### ❌ UI-Elemente überlappen
**Das ist normal!**
- Passe die Ladereihenfolge der Pakete an
- Manche UI-Anpassungen sind inkompatibel

---

## 💡 Tipps

### Tipp 1: Als .mcpack speichern
Für einfachere Installation:
```bash
cd larger_hotbar_pack
zip -r ../larger_hotbar_pack.mcpack *
```
Dann einfach die .mcpack Datei öffnen!

### Tipp 2: Pack-Icon hinzufügen
1. Erstelle ein 256x256 PNG Bild
2. Nenne es `pack_icon.png`
3. Lege es in den `larger_hotbar_pack` Ordner
4. Fertig!

### Tipp 3: Verschiedene Größen erstellen
Erstelle mehrere Kopien mit verschiedenen Größen:
- `hotbar_small` (25% größer)
- `hotbar_medium` (50% größer) ← aktuell
- `hotbar_large` (100% größer)
- `hotbar_xl` (150% größer)

**Wichtig:** Ändere die UUIDs für jede Kopie!

---

## 🆔 Einzigartige UUIDs

Dieses Paket verwendet diese UUIDs:
- **Header**: `6423d417-3bfa-4f02-9261-a4503fa8049d`
- **Module**: `5b355b56-eee8-46f9-808b-3bb398b599d9`

**Wenn du das Paket modifizierst und weitergibst:**  
Generiere neue UUIDs auf: https://www.uuidgenerator.net/

---

## 📝 Lizenz

Dieses Ressourcenpaket ist frei verwendbar. Du kannst es:
- ✅ Verwenden
- ✅ Modifizieren
- ✅ Weitergeben
- ✅ In eigenen Projekten nutzen

Bedingung: Generiere neue UUIDs wenn du es weitergibst!

---

## 🌐 Unterstützte Plattformen

- ✅ Windows 10/11
- ✅ Android
- ✅ iOS
- ✅ Xbox
- ✅ PlayStation
- ✅ Nintendo Switch

**Voraussetzung:** Minecraft Bedrock Edition 1.21.0 oder neuer

---

## ❓ Häufige Fragen

**F: Funktioniert das auch in Java Edition?**  
A: Nein, nur für Bedrock Edition.

**F: Kann ich die Farbe der Hotbar ändern?**  
A: Dafür brauchst du Textur-Dateien, nicht nur UI-Dateien.

**F: Funktioniert es im Mehrspieler?**  
A: Ja, aber nur du siehst die größere Hotbar.

**F: Kann ich mehrere Ressourcenpakete verwenden?**  
A: Ja, aber achte auf die Ladereihenfolge.

**F: Wie deinstalliere ich das Paket?**  
A: Deaktiviere es in "Globale Ressourcen" oder lösche den Ordner.

---

## 🎯 Zusammenfassung

✅ **Einfache Installation** - Nur Ordner kopieren  
✅ **Sofort einsatzbereit** - Keine Konfiguration nötig  
✅ **Anpassbar** - Größe nach Wunsch ändern  
✅ **Sicher** - Einzigartige UUIDs  
✅ **Kompatibel** - Alle Plattformen  

**Viel Spaß mit deiner größeren Hotbar! 🎮**
