# Custom Hotbar Size Resource Pack

Dieses Resource Pack vergrößert die Hotbar in Minecraft Bedrock Edition oder ermöglicht es Ihnen, die Größe nach Ihren Wünschen anzupassen.

## Installation

1. Kopieren Sie den gesamten Ordner `custom_hotbar_pack` in Ihren Minecraft-Ressourcenpakete-Ordner:
   - **Windows**: `%localappdata%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs\`
   - **Android**: `sdcard/games/com.mojang/resource_packs/`
   - **iOS**: `On My iPhone/Minecraft/games/com.mojang/resource_packs/`
   
2. Starten Sie Minecraft Bedrock Edition
3. Gehen Sie zu Einstellungen → Globale Ressourcen
4. Aktivieren Sie "Custom Hotbar Size"

## Anpassung der Hotbar-Größe

Um die Hotbar-Größe anzupassen, bearbeiten Sie die Datei `ui/hud_screen.json`:

### Desktop/PC (Standard 20x22):
```json
"hotbar_renderer": {
  "$hotbar_renderer_size|default": [ 30, 33 ],  // Breite, Höhe (aktuell 150% der Originalgröße)
  ...
}
```

### Mobile/Pocket Edition (Standard 40):
```json
"hotbar_panel_pocket": {
  "size": [ "100%", 60 ],  // Höhe (aktuell 150% der Originalgröße)
  ...
}
```

### Empfohlene Größen:

**Desktop:**
- **Klein (75%)**: `[ 15, 16.5 ]`
- **Normal (100%)**: `[ 20, 22 ]`
- **Groß (125%)**: `[ 25, 27.5 ]`
- **Sehr groß (150%)**: `[ 30, 33 ]` ← Aktuell eingestellt
- **Riesig (200%)**: `[ 40, 44 ]`

**Pocket:**
- **Klein (75%)**: `30`
- **Normal (100%)**: `40`
- **Groß (125%)**: `50`
- **Sehr groß (150%)**: `60` ← Aktuell eingestellt
- **Riesig (200%)**: `80`

## Struktur des Resource Packs

```
custom_hotbar_pack/
├── manifest.json          # Pack-Metadaten und UUIDs
├── pack_icon.png          # Pack-Symbol (optional)
├── README.md              # Diese Datei
└── ui/
    └── hud_screen.json    # Hotbar-Größenkonfiguration
```

## Technische Details

- **Format Version**: 2
- **Minimale Engine Version**: 1.21.0
- **UUIDs**: Einzigartig generiert für dieses Pack
  - Header UUID: `4b84ef0b-9a8f-40fb-b07a-82a7fa8a13a5`
  - Module UUID: `d6d2daaa-2b90-42c6-ac72-17a16a533ad5`

## Hinweise

- Die Hotbar-Größe wird sowohl für Desktop als auch für Pocket Edition (Mobile) angepasst
- Die XP-Leiste und andere UI-Elemente werden automatisch angepasst
- Die Änderungen sind nur visuell und beeinflussen nicht das Gameplay
- Sie können die Größe jederzeit durch Bearbeiten der `hud_screen.json` anpassen

## Fehlerbehebung

**Das Pack wird nicht angezeigt:**
- Stellen Sie sicher, dass der Ordner im richtigen Verzeichnis liegt
- Überprüfen Sie, ob die `manifest.json` keine Syntaxfehler hat

**Die Hotbar ist zu groß/klein:**
- Bearbeiten Sie die Werte in `ui/hud_screen.json` wie oben beschrieben
- Starten Sie die Welt neu, um Änderungen zu übernehmen

**Konflikte mit anderen Packs:**
- Dieses Pack überschreibt nur die Hotbar-Elemente in `hud_screen.json`
- Packs mit höherer Priorität können diese Änderungen überschreiben

## Lizenz

Dieses Resource Pack ist frei verwendbar und kann nach Belieben angepasst werden.
