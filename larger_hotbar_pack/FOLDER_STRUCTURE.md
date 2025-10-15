# Ordnerstruktur des Ressourcenpakets / Resource Pack Folder Structure

## Vollständige Ordnerstruktur / Complete Folder Structure

```
larger_hotbar_pack/
├── manifest.json                    (Paket-Metadaten / Pack metadata)
├── README.md                        (Englische Anleitung / English guide)
├── README_DE.md                     (Deutsche Anleitung / German guide)
├── pack_icon_instructions.txt       (Anweisungen für Icon / Icon instructions)
└── ui/
    └── hud_screen.json             (Hotbar UI-Modifikationen / Hotbar UI modifications)
```

## Dateibeschreibungen / File Descriptions

### manifest.json
**Zweck / Purpose**: Definiert das Ressourcenpaket und seine Metadaten  
**Wichtig / Important**: Enthält einzigartige UUIDs  
**Bearbeiten / Edit**: Nur wenn du Name, Beschreibung oder Version ändern möchtest

### ui/hud_screen.json
**Zweck / Purpose**: Enthält die Hotbar-Größen-Modifikationen  
**Wichtig / Important**: Hier kannst du die Größe anpassen  
**Bearbeiten / Edit**: Um verschiedene Hotbar-Größen zu erstellen

### README.md / README_DE.md
**Zweck / Purpose**: Installations- und Nutzungsanleitung  
**Wichtig / Important**: Hilft Benutzern das Paket zu installieren  
**Bearbeiten / Edit**: Optional, wenn du zusätzliche Informationen hinzufügen möchtest

## Verwendung / Usage

### Schritt 1: Ordner kopieren / Step 1: Copy Folder
Kopiere den gesamten `larger_hotbar_pack` Ordner in dein Minecraft Ressourcenpakete-Verzeichnis.

Copy the entire `larger_hotbar_pack` folder to your Minecraft resource packs directory.

### Schritt 2: In Minecraft aktivieren / Step 2: Activate in Minecraft
- Öffne Minecraft / Open Minecraft
- Gehe zu Einstellungen > Globale Ressourcen / Go to Settings > Global Resources
- Aktiviere das Paket / Activate the pack

### Schritt 3: Optional - Als ZIP verpacken / Step 3: Optional - Package as ZIP
Falls gewünscht, kannst du den Ordner auch als .mcpack oder .zip Datei verpacken:

If desired, you can package the folder as .mcpack or .zip file:

```bash
# Als ZIP (umbenennen zu .mcpack für einfache Installation)
# As ZIP (rename to .mcpack for easy installation)
cd larger_hotbar_pack
zip -r ../larger_hotbar_pack.zip *
# Dann umbenennen / Then rename: larger_hotbar_pack.zip -> larger_hotbar_pack.mcpack
```

## Anpassung der Größe / Size Customization

In `ui/hud_screen.json` findest du folgende Größenwerte, die du ändern kannst:

In `ui/hud_screen.json` you will find the following size values you can change:

| Element | Standard / Default | Aktuell / Current | Zweck / Purpose |
|---------|-------------------|-------------------|-----------------|
| `hotbar_renderer_size` | `[20, 22]` | `[30, 33]` | Slot-Renderer / Slot renderer |
| `gui_hotbar_grid_item` | `[20, 22]` | `[30, 33]` | Grid-Item-Größe / Grid item size |
| `item_icon` | `[16, 16]` | `[24, 24]` | Item-Icon-Größe / Item icon size |
| `hotbar_slot_selected_image` | `[24, 24]` | `[36, 36]` | Ausgewählter Slot / Selected slot |
| `hotbar_panel` | `22` (Höhe) | `33` (Höhe) | Panel-Höhe / Panel height |

## Einzigartige UUIDs / Unique UUIDs

Dieses Paket verwendet die folgenden einzigartigen UUIDs:
This pack uses the following unique UUIDs:

- **Header UUID**: `6423d417-3bfa-4f02-9261-a4503fa8049d`
- **Module UUID**: `5b355b56-eee8-46f9-808b-3bb398b599d9`

⚠️ **Wichtig / Important**: Wenn du dieses Paket als Basis für dein eigenes Paket verwendest, generiere neue UUIDs!  
⚠️ **Important**: If you use this pack as a base for your own pack, generate new UUIDs!

### Neue UUIDs generieren / Generate New UUIDs

```python
import uuid
print(f"Header UUID: {uuid.uuid4()}")
print(f"Module UUID: {uuid.uuid4()}")
```

Oder online: https://www.uuidgenerator.net/

## Fehlerbehebung / Troubleshooting

**Problem**: Hotbar wird nicht größer  
**Solution**: Überprüfe ob das Paket aktiviert ist und starte Minecraft neu

**Problem**: Hotbar doesn't get larger  
**Solution**: Check if the pack is activated and restart Minecraft

---

**Problem**: Andere UI-Elemente überlappen  
**Solution**: Passe die Ladereihenfolge der Ressourcenpakete an

**Problem**: Other UI elements overlap  
**Solution**: Adjust the resource pack load order

---

**Problem**: Funktioniert nicht auf meiner Plattform  
**Solution**: Stelle sicher, dass du Minecraft Bedrock Edition 1.21.0+ verwendest

**Problem**: Doesn't work on my platform  
**Solution**: Make sure you're using Minecraft Bedrock Edition 1.21.0+

## Support

Für weitere Hilfe oder Fragen:  
For further help or questions:

- Lies die README.md / Read the README.md
- Überprüfe die Minecraft Bedrock Dokumentation / Check the Minecraft Bedrock documentation
- Frage in Minecraft Community-Foren / Ask in Minecraft community forums
