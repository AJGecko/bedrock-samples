# Custom Hotbar Size Resource Pack - Overview

## Übersicht (German)

Dieses Resource Pack wurde erstellt, um die Hotbar in Minecraft Bedrock Edition zu vergrößern und anpassbar zu machen.

### Hauptmerkmale:
✅ Vergrößert die Hotbar um 50% (von 20x22 auf 30x33 Pixel für Desktop)
✅ Vergrößert die mobile Hotbar um 50% (von 40 auf 60 Pixel)
✅ Vollständig anpassbar durch Bearbeitung einer einzigen Datei
✅ Eindeutige UUIDs zur Vermeidung von Konflikten
✅ Kompatibel mit Minecraft Bedrock 1.21.0+
✅ Funktioniert auf Desktop, Mobile und Konsolen

### Paketinhalt:
```
custom_hotbar_pack/
├── INSTALLATION.md       - Zweisprachige Installationsanleitung
├── QUICK_REFERENCE.md    - Schnellreferenz für Größenanpassungen
├── README.md             - Ausführliche Dokumentation (Deutsch)
├── manifest.json         - Pack-Metadaten mit eindeutigen UUIDs
├── pack_icon.png         - Pack-Symbol
└── ui/
    └── hud_screen.json   - Hotbar-Größenkonfiguration
```

---

## Overview (English)

This resource pack was created to make the hotbar in Minecraft Bedrock Edition larger and customizable.

### Key Features:
✅ Enlarges hotbar by 50% (from 20x22 to 30x33 pixels for desktop)
✅ Enlarges mobile hotbar by 50% (from 40 to 60 pixels)
✅ Fully customizable by editing a single file
✅ Unique UUIDs to prevent conflicts
✅ Compatible with Minecraft Bedrock 1.21.0+
✅ Works on Desktop, Mobile, and Consoles

### Pack Contents:
```
custom_hotbar_pack/
├── INSTALLATION.md       - Bilingual installation guide
├── QUICK_REFERENCE.md    - Quick reference for size adjustments
├── README.md             - Detailed documentation (German)
├── manifest.json         - Pack metadata with unique UUIDs
├── pack_icon.png         - Pack icon
└── ui/
    └── hud_screen.json   - Hotbar size configuration
```

---

## Technical Details / Technische Details

### UUIDs (Do not modify / Nicht ändern):
- **Header UUID**: `4b84ef0b-9a8f-40fb-b07a-82a7fa8a13a5`
- **Module UUID**: `d6d2daaa-2b90-42c6-ac72-17a16a533ad5`

### Modified Files / Geänderte Dateien:
- `ui/hud_screen.json` - Overrides the vanilla HUD screen to increase hotbar size

### Size Parameters / Größenparameter:

**Desktop/PC:**
- Hotbar renderer: 30x33 pixels (default: 20x22)
- Cooldown renderer: 30x33 pixels (default: 20x22)
- Panel height: 33 pixels (default: 22)
- XP bar offset: 24 pixels (default: 16)

**Mobile/Pocket:**
- Panel height: 60 pixels (default: 40)

### Customization / Anpassung:

All customization is done in `ui/hud_screen.json`:
- Lines 7, 44: Desktop hotbar size
- Line 52: Desktop panel height
- Line 73: Mobile panel height
- Lines 258, 282, 308: Hotbar Y-offset (increase for larger hotbars)

---

## Installation Paths / Installationspfade

**Windows 10/11:**
```
%localappdata%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs\custom_hotbar_pack\
```

**Android:**
```
/sdcard/games/com.mojang/resource_packs/custom_hotbar_pack/
```

**iOS:**
```
On My iPhone/Minecraft/games/com.mojang/resource_packs/custom_hotbar_pack/
```

---

## Quick Start / Schnellstart

1. Copy `custom_hotbar_pack` folder to resource packs directory
   Kopieren Sie den Ordner `custom_hotbar_pack` in das Ressourcenpakete-Verzeichnis

2. Launch Minecraft / Minecraft starten

3. Settings → Global Resources → Activate "Custom Hotbar Size"
   Einstellungen → Globale Ressourcen → "Custom Hotbar Size" aktivieren

4. Enjoy your larger hotbar!
   Genießen Sie Ihre größere Hotbar!

---

## Support / Unterstützung

For issues or questions:
- Check QUICK_REFERENCE.md for common adjustments
- Verify JSON syntax if making manual edits
- Ensure UUIDs remain unique

Bei Problemen oder Fragen:
- Prüfen Sie QUICK_REFERENCE.md für häufige Anpassungen
- Überprüfen Sie die JSON-Syntax bei manuellen Änderungen
- Stellen Sie sicher, dass UUIDs eindeutig bleiben

---

**Pack Size / Paketgröße**: ~68 KB
**Format Version**: 2
**Minimum Engine**: 1.21.0
