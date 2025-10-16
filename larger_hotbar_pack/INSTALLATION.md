# Installations-Anleitung / Installation Guide

## Deutsch

### Schnelle Installation (Empfohlen)

1. **Ordner auf dein Gerät kopieren**
   - Kopiere den kompletten `larger_hotbar_pack` Ordner auf dein Smartphone/Tablet

2. **Ordner verschieben**
   
   **Android:**
   ```
   Interner Speicher/Android/data/com.mojang.minecraftpe/files/games/com.mojang/resource_packs/larger_hotbar_pack/
   ```
   
   **iOS:**
   ```
   Auf meinem iPhone/Minecraft PE/games/com.mojang/resource_packs/larger_hotbar_pack/
   ```

3. **Minecraft starten**
   - Öffne Minecraft Bedrock Edition
   - Gehe zu: Einstellungen → Globale Ressourcen
   - Klicke auf "Meine Packs"
   - Finde "Größere Hotbar Pack" in der Liste
   - Klicke auf "+" um es zu aktivieren
   - Fertig!

### Alternative: .mcpack Installation

1. **Ordner umbenennen**
   - Benenne den Ordner `larger_hotbar_pack` in `larger_hotbar_pack.mcpack` um

2. **Datei öffnen**
   - Tippe auf die `.mcpack` Datei
   - Minecraft öffnet sich automatisch

3. **Aktivieren**
   - Das Pack wird automatisch importiert
   - Gehe zu Einstellungen → Globale Ressourcen
   - Aktiviere das Pack

### Was wird größer?

✓ Hotbar (50% größer)
✓ Herzen/Leben (50% größer)
✓ Hunger-Bar (50% größer)
✓ Rüstungsanzeige (50% größer)
✓ XP-Bar (50% größer)
✓ Luft-Blasen (50% größer)

### Alle Buttons funktionieren!

✓ Inventar-Button
✓ Crafting-Button
✓ Hotbar-Navigation (Elipsen)
✓ Alle Slot-Hitboxen sind korrekt

---

## English

### Quick Installation (Recommended)

1. **Copy folder to your device**
   - Copy the complete `larger_hotbar_pack` folder to your smartphone/tablet

2. **Move folder to**
   
   **Android:**
   ```
   Internal Storage/Android/data/com.mojang.minecraftpe/files/games/com.mojang/resource_packs/larger_hotbar_pack/
   ```
   
   **iOS:**
   ```
   On My iPhone/Minecraft PE/games/com.mojang/resource_packs/larger_hotbar_pack/
   ```

3. **Start Minecraft**
   - Open Minecraft Bedrock Edition
   - Go to: Settings → Global Resources
   - Click on "My Packs"
   - Find "Größere Hotbar Pack" in the list
   - Click "+" to activate it
   - Done!

### Alternative: .mcpack Installation

1. **Rename folder**
   - Rename the folder `larger_hotbar_pack` to `larger_hotbar_pack.mcpack`

2. **Open file**
   - Tap on the `.mcpack` file
   - Minecraft will open automatically

3. **Activate**
   - The pack will be imported automatically
   - Go to Settings → Global Resources
   - Activate the pack

### What gets bigger?

✓ Hotbar (50% larger)
✓ Hearts/Health (50% larger)
✓ Hunger Bar (50% larger)
✓ Armor Display (50% larger)
✓ XP Bar (50% larger)
✓ Air Bubbles (50% larger)

### All buttons work!

✓ Inventory button
✓ Crafting button
✓ Hotbar navigation (ellipses)
✓ All slot hitboxes are correct

---

## Troubleshooting / Problemlösung

### Pack wird nicht angezeigt / Pack not showing

**DE:** Stelle sicher, dass der Ordner die richtige Struktur hat:
```
larger_hotbar_pack/
├── manifest.json
├── pack_icon.png
├── README.md
└── ui/
    ├── _ui_defs.json
    ├── _global_variables.json
    └── hud_screen.json
```

**EN:** Make sure the folder has the correct structure (see above)

### UI-Elemente sind zu groß / UI elements too big

**DE:** Du kannst die Skalierung in `ui/hud_screen.json` anpassen (suche nach den Zahlen 1.5, 30, 33, 60 und 7.5)

**EN:** You can adjust scaling in `ui/hud_screen.json` (look for numbers 1.5, 30, 33, 60, and 7.5)

### Konflikte mit anderen Packs / Conflicts with other packs

**DE:** Stelle sicher, dass dieses Pack in der Liste der Ressourcenpacks über anderen UI-Packs steht

**EN:** Make sure this pack is above other UI packs in the resource pack list
