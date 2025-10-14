# Größere Hotbar Ressourcenpaket

Dieses Ressourcenpaket macht die Hotbar in Minecraft Bedrock Edition größer für bessere Sichtbarkeit.

## Funktionen

- **Größere Hotbar-Slots**: Die Hotbar-Slots werden von 20x22 Pixel auf 30x33 Pixel vergrößert (50% größer)
- **Größere Item-Icons**: Item-Icons werden von 16x16 auf 24x24 Pixel skaliert
- **Größerer ausgewählter Slot-Indikator**: Der Rahmen des ausgewählten Slots wird von 24x24 auf 36x36 Pixel vergrößert
- **Alle Elemente proportional skaliert**: Enthält Kappen, Buttons und andere UI-Elemente

## Installation

1. Kopiere den gesamten `larger_hotbar_pack` Ordner in deinen Minecraft Ressourcenpakete-Ordner:
   - **Windows**: `%localappdata%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs\`
   - **Android**: `/storage/emulated/0/games/com.mojang/resource_packs/`
   - **iOS**: `Apps/com.mojang.minecraftpe/Documents/games/com.mojang/resource_packs/`

2. Öffne Minecraft Bedrock Edition

3. Gehe zu **Einstellungen** > **Globale Ressourcen**

4. Finde "Larger Hotbar Resource Pack" in der Liste verfügbarer Pakete

5. Klicke auf den **+** Button um es zu aktivieren

6. Klicke auf **Anwenden** oder starte das Spiel neu, falls nötig

## Anpassung

Um die Hotbar-Größe anzupassen, bearbeite die Datei `ui/hud_screen.json` und ändere die Größenwerte:

- **Standardgröße**: `[ 20, 22 ]` (Breite, Höhe in Pixel)
- **Aktuelle Größe**: `[ 30, 33 ]` (50% größer)

Du kannst diese Werte auf jede beliebige Größe ändern. Zum Beispiel:
- **75% größer**: `[ 35, 38.5 ]`
- **100% größer**: `[ 40, 44 ]`
- **25% größer**: `[ 25, 27.5 ]`

Stelle sicher, dass du alle Instanzen in der Datei aktualisierst für konsistente Skalierung:
- `hotbar_renderer_size`
- `gui_hotbar_grid_item` Größe
- `hotbar_slot_image_size`
- `hotbar_panel` Größe
- Item-Icon-Größen
- Größe des ausgewählten Slot-Indikators

## Technische Details

**Format-Version**: 2  
**Minimale Engine-Version**: 1.21.0

**UUIDs**:
- Header: `6423d417-3bfa-4f02-9261-a4503fa8049d`
- Modul: `5b355b56-eee8-46f9-808b-3bb398b599d9`

Diese UUIDs sind einzigartig für dieses Ressourcenpaket und stellen sicher, dass es nicht mit anderen Paketen in Konflikt gerät.

## Kompatibilität

- Funktioniert mit Minecraft Bedrock Edition Version 1.21.0 und neuer
- Kompatibel mit anderen Ressourcenpaketen (Ladereihenfolge kann wichtig sein)
- Sollte auf allen Plattformen funktionieren (Windows, Android, iOS, Xbox, PlayStation, Nintendo Switch)

## Fehlerbehebung

**Hotbar ändert die Größe nicht:**
- Stelle sicher, dass das Ressourcenpaket in Einstellungen > Globale Ressourcen aktiviert ist
- Versuche Minecraft neu zu starten
- Überprüfe, dass kein anderes Ressourcenpaket die Hotbar-UI überschreibt

**UI-Elemente nicht ausgerichtet:**
- Das ist zu erwarten, wenn es mit bestimmten benutzerdefinierten UIs verwendet wird
- Passe die Ladereihenfolge der Ressourcenpakete im Menü Globale Ressourcen an

## Lizenz

Dieses Ressourcenpaket wird wie besehen zur Verwendung mit Minecraft Bedrock Edition bereitgestellt. Du darfst es frei modifizieren und weiterverbreiten.
