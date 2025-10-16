# Größere Hotbar Resource Pack für Minecraft Bedrock Edition (Pocket/Mobile)

## Beschreibung
Dieses Resource Pack vergrößert die Hotbar und alle zugehörigen HUD-Elemente für Minecraft Bedrock Edition auf Mobilgeräten (Pocket Edition) um das 1,5-fache.

## Änderungen
- **Hotbar**: 1,5x größer (von 40px auf 60px Höhe)
- **Herzen (Hearts)**: 1,5x größer
- **Hunger-Anzeige**: 1,5x größer
- **Rüstungs-Anzeige (Armor)**: 1,5x größer
- **Pferde-Herzen**: 1,5x größer
- **Sauerstoff-Blasen (Bubbles)**: 1,5x größer
- **XP-Bar**: Korrekt positioniert unter der größeren Hotbar
- **Item-Icons in der Hotbar**: Größer (85% statt 80%)

## Installation

### Auf Android-Geräten:
1. Lade den `larger_hotbar_pack` Ordner herunter
2. Öffne einen Dateimanager auf deinem Android-Gerät
3. Navigiere zu: `/storage/emulated/0/games/com.mojang/resource_packs/`
4. Kopiere den gesamten `larger_hotbar_pack` Ordner in diesen Ordner
5. Starte Minecraft Bedrock Edition
6. Gehe zu Einstellungen → Globale Ressourcen
7. Aktiviere "Größere Hotbar Pack"

### Auf iOS-Geräten:
1. Lade den `larger_hotbar_pack` Ordner herunter
2. Verwende eine App wie "Documents by Readdle" oder eine ähnliche Dateimanager-App
3. Navigiere zu: `Minecraft/games/com.mojang/resource_packs/`
4. Kopiere den gesamten `larger_hotbar_pack` Ordner in diesen Ordner
5. Starte Minecraft Bedrock Edition
6. Gehe zu Einstellungen → Globale Ressourcen
7. Aktiviere "Größere Hotbar Pack"

### Auf Windows 10/11 (für Tests):
1. Drücke `Windows + R`
2. Gib ein: `%localappdata%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs`
3. Kopiere den `larger_hotbar_pack` Ordner hierher
4. Starte Minecraft und aktiviere das Pack in den Einstellungen

## Funktionalität
- ✅ Alle Inventar-Buttons funktionieren weiterhin
- ✅ Hotbar-Slot-Hitboxen sind korrekt angepasst
- ✅ Items können normal aufgenommen und verwendet werden
- ✅ Alle Touch-Steuerungen funktionieren normal
- ✅ Kompatibel mit allen Spielmodi (Überleben, Kreativ, Abenteuer)

## Technische Details
- Format Version: 2
- Minimum Engine Version: 1.20.0
- Pack Version: 1.0.0
- Typ: Resource Pack (nur clientseitig)

## Anpassungen
Das Pack modifiziert folgende UI-Elemente:
- `hud_screen.json` - Hauptdatei für alle HUD-Änderungen
  - `hotbar_panel_pocket` - Vergrößerte Hotbar-Größe
  - `gui_hotbar_grid_item_pocket` - Vergrößerte Item-Icons
  - `exp_progress_bar_and_hotbar` - Angepasste XP-Bar-Position
  - `heart_renderer` - Vergrößerte Herzen
  - `hunger_renderer` - Vergrößerte Hunger-Anzeige
  - `armor_renderer` - Vergrößerte Rüstungs-Anzeige
  - `horse_heart_renderer` - Vergrößerte Pferde-Herzen
  - `bubbles_renderer` - Vergrößerte Sauerstoff-Anzeige

## Kompatibilität
- ✅ Minecraft Bedrock Edition 1.20.0+
- ✅ Android
- ✅ iOS
- ✅ Windows 10/11 (UWP)
- ✅ Funktioniert mit anderen Resource Packs (solange diese nicht die gleichen UI-Elemente ändern)

## Hinweise
- Dieses Pack ändert nur die Größe der UI-Elemente, keine Texturen
- Alle Standard-Texturen von Minecraft werden verwendet
- Das Pack ist optimiert für Touchscreen-Geräte (Pocket Edition)
- Bei kleineren Bildschirmen könnte die Hotbar viel Platz einnehmen - in diesem Fall kann das Pack einfach deaktiviert werden

## Lizenz
Dieses Resource Pack basiert auf den offiziellen Minecraft Bedrock Samples und dient nur zu Demonstrationszwecken.
