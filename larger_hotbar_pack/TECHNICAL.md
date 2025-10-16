# Technische Spezifikationen / Technical Specifications

## Geänderte Elemente / Modified Elements

### Hotbar

#### Standard / Default:
- Slot-Größe: 20x22 Pixel
- Panel-Höhe: 40 Pixel
- Renderer-Größe: 20x22

#### Mit diesem Pack / With this pack:
- Slot-Größe: 30x33 Pixel (+50%)
- Panel-Höhe: 60 Pixel (+50%)
- Renderer-Größe: 30x33

### Herzen / Hearts

#### Standard / Default:
- Renderer-Größe: 1x1

#### Mit diesem Pack / With this pack:
- Renderer-Größe: 1.5x1.5 (+50%)

### Hunger-Bar / Hunger Bar

#### Standard / Default:
- Renderer-Größe: 1x1

#### Mit diesem Pack / With this pack:
- Renderer-Größe: 1.5x1.5 (+50%)

### Rüstung / Armor

#### Standard / Default:
- Renderer-Größe: 1x1

#### Mit diesem Pack / With this pack:
- Renderer-Größe: 1.5x1.5 (+50%)

### XP-Bar / Experience Bar

#### Standard / Default:
- Höhe: 5 Pixel

#### Mit diesem Pack / With this pack:
- Höhe: 7.5 Pixel (+50%)

### Luft-Blasen / Air Bubbles

#### Standard / Default:
- Renderer-Größe: 1x1

#### Mit diesem Pack / With this pack:
- Renderer-Größe: 1.5x1.5 (+50%)

## Datei-Struktur / File Structure

```
larger_hotbar_pack/
│
├── manifest.json                    # Pack-Metadaten / Pack metadata
├── pack_icon.png                    # Pack-Symbol / Pack icon
├── README.md                        # Hauptdokumentation / Main documentation
├── INSTALLATION.md                  # Installationsanleitung / Installation guide
├── TECHNICAL.md                     # Diese Datei / This file
│
├── ui/                             # UI-Definitionen / UI definitions
│   ├── _ui_defs.json              # UI-Registrierung / UI registration
│   ├── _global_variables.json     # Globale Variablen / Global variables
│   └── hud_screen.json            # HUD-Modifikationen / HUD modifications
│
└── textures/                       # Texturen (optional) / Textures (optional)
    └── ui/                        # UI-Texturen / UI textures
```

## Modifizierte JSON-Elemente / Modified JSON Elements

### hud_screen.json

Die folgenden Elemente wurden modifiziert / The following elements were modified:

1. **hotbar_renderer**
   - Größe: `[ 30, 33 ]` (war `[ 20, 22 ]`)
   - Beschreibung: Rendert die einzelnen Hotbar-Slots

2. **cooldown_renderer**
   - Größe: `[ 30, 33 ]` (war `[ 20, 22 ]`)
   - Beschreibung: Rendert die Abklingzeit-Anzeige für Items

3. **heart_renderer**
   - Größe: `[ 1.5, 1.5 ]` (war `[ 1, 1 ]`)
   - Beschreibung: Rendert die Lebensherzen

4. **horse_heart_renderer**
   - Größe: `[ 1.5, 1.5 ]` (war `[ 1, 1 ]`)
   - Beschreibung: Rendert die Pferde-Lebensherzen

5. **armor_renderer**
   - Größe: `[ 1.5, 1.5 ]` (war `[ 1, 1 ]`)
   - Beschreibung: Rendert die Rüstungspunkte

6. **hunger_renderer**
   - Größe: `[ 1.5, 1.5 ]` (war `[ 1, 1 ]`)
   - Beschreibung: Rendert die Hunger-Punkte

7. **bubble_renderer**
   - Größe: `[ 1.5, 1.5 ]` (war `[ 1, 1 ]`)
   - Beschreibung: Rendert die Luft-Blasen unter Wasser

8. **hotbar_panel_pocket**
   - Panel-Höhe: `60` (war `40`)
   - Start-Cap-Größe: `[ 1.5, "100%" ]` (war `[ 1, "100%" ]`)
   - End-Cap-Größe: `[ 1.5, "100%" ]` (war `[ 1, "100%" ]`)
   - Beschreibung: Das gesamte Hotbar-Panel für Pocket Edition

9. **exp_progress_bar_and_hotbar_pocket**
   - XP-Bar-Höhe: `7.5` (war `5`)
   - Locator-Bar-Höhe: `7.5` (war `5`)
   - Horse-Jump-Bar-Höhe: `7.5` (war `5`)
   - Dash-Bar-Höhe: `7.5` (war `5`)
   - Beschreibung: Die Erfahrungsleiste und alternative Bars

## Kompatibilität / Compatibility

### Funktioniert mit / Works with:
- ✓ Vanilla Minecraft Bedrock
- ✓ Realms
- ✓ Multiplayer-Server
- ✓ Alle Spielmodi (Überleben, Kreativ, Abenteuer)
- ✓ Anderen Ressourcenpacks (solange sie nicht die HUD ändern)

### Funktioniert NICHT mit / Does NOT work with:
- ✗ Anderen HUD-modifizierenden Packs (Konflikte möglich)
- ✗ Minecraft Java Edition (nur für Bedrock)

## Anpassung / Customization

### Skalierungsfaktor ändern / Change scaling factor

Um die Vergrößerung anzupassen, ändere die Werte in `ui/hud_screen.json`:

To adjust the scaling, change the values in `ui/hud_screen.json`:

**Für 2x Vergrößerung / For 2x scaling:**
- Hotbar: `[ 40, 44 ]`
- Hearts/Hunger/Armor/Bubbles: `[ 2, 2 ]`
- XP-Bar: `10`
- Panel-Höhe: `80`

**Für 1.25x Vergrößerung / For 1.25x scaling:**
- Hotbar: `[ 25, 27.5 ]`
- Hearts/Hunger/Armor/Bubbles: `[ 1.25, 1.25 ]`
- XP-Bar: `6.25`
- Panel-Höhe: `50`

## Leistung / Performance

- **Keine Auswirkung auf FPS** / No impact on FPS
- **Keine zusätzlichen Texturen geladen** / No additional textures loaded
- **Nur UI-Layout-Änderungen** / Only UI layout changes
- **Kompatibel mit allen Geräten** / Compatible with all devices

## Bekannte Einschränkungen / Known Limitations

1. **Bildschirmplatz** / Screen space
   - Auf kleinen Bildschirmen kann die vergrößerte UI mehr Platz einnehmen
   - On small screens, the enlarged UI may take up more space

2. **Tablet-Modus** / Tablet mode
   - Optimiert für Handy (Pocket Edition Touch-Controls)
   - Optimized for phones (Pocket Edition touch controls)

3. **Textur-Skalierung** / Texture scaling
   - Standard-Texturen werden von Minecraft automatisch skaliert
   - Default textures are automatically scaled by Minecraft
   - Für beste Qualität könnten höher aufgelöste Texturen hinzugefügt werden
   - For best quality, higher resolution textures could be added

## Version-Historie / Version History

### v1.0.0 (2025-10-16)
- Erste Veröffentlichung / Initial release
- 50% Vergrößerung aller HUD-Elemente / 50% scaling of all HUD elements
- Pocket Edition Unterstützung / Pocket Edition support
- Vollständig funktionsfähige UI-Buttons / Fully functional UI buttons
