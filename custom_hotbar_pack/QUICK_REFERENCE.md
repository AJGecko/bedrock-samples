# QUICK REFERENCE - SCHNELLREFERENZ

## How to Change Hotbar Size / Wie man die Hotbar-Größe ändert

### File to Edit / Zu bearbeitende Datei:
`ui/hud_screen.json`

---

## Desktop/PC Hotbar Size / Desktop/PC Hotbar-Größe

**Line 7 / Zeile 7:**
```json
"$hotbar_renderer_size|default": [ WIDTH, HEIGHT ],
```

**Line 44 / Zeile 44:**
```json
"size": [ WIDTH, HEIGHT ],
```

**Line 52 / Zeile 52:**
```json
"size": [ "100%c", HEIGHT ],
```

### Quick Copy-Paste Values / Schnelle Kopier-Einfügen-Werte:

**50% Smaller / 50% kleiner:**
- `[ 10, 11 ]` for lines 7 and 44
- `[ "100%c", 11 ]` for line 52

**25% Smaller / 25% kleiner:**
- `[ 15, 16.5 ]` for lines 7 and 44
- `[ "100%c", 16.5 ]` for line 52

**Default / Standard (100%):**
- `[ 20, 22 ]` for lines 7 and 44
- `[ "100%c", 22 ]` for line 52

**25% Larger / 25% größer:**
- `[ 25, 27.5 ]` for lines 7 and 44
- `[ "100%c", 27.5 ]` for line 52

**50% Larger / 50% größer (CURRENT / AKTUELL):**
- `[ 30, 33 ]` for lines 7 and 44
- `[ "100%c", 33 ]` for line 52

**100% Larger / 100% größer:**
- `[ 40, 44 ]` for lines 7 and 44
- `[ "100%c", 44 ]` for line 52

---

## Mobile/Pocket Hotbar Size / Mobile/Pocket Hotbar-Größe

**Line 73 / Zeile 73:**
```json
"size": [ "100%", HEIGHT ],
```

### Quick Copy-Paste Values / Schnelle Kopier-Einfügen-Werte:

**50% Smaller:** `[ "100%", 20 ]`
**25% Smaller:** `[ "100%", 30 ]`
**Default (100%):** `[ "100%", 40 ]`
**25% Larger:** `[ "100%", 50 ]`
**50% Larger (CURRENT):** `[ "100%", 60 ]`
**100% Larger:** `[ "100%", 80 ]`

---

## Important Notes / Wichtige Hinweise

1. **Always maintain the aspect ratio** / **Behalten Sie immer das Seitenverhältnis bei**
   - Desktop width:height ratio is approximately 20:22 (or 0.909)
   - Desktop Breite:Höhe Verhältnis ist ungefähr 20:22 (oder 0.909)

2. **After editing, reload the world** / **Nach der Bearbeitung die Welt neu laden**
   - Save and exit the world
   - Re-enter to see changes
   - Welt speichern und verlassen
   - Erneut betreten, um Änderungen zu sehen

3. **Line numbers for key sections** / **Zeilennummern für wichtige Abschnitte:**
   - Line 7: Desktop hotbar renderer size
   - Line 44: Desktop cooldown renderer size  
   - Line 52: Desktop hotbar panel height
   - Line 73: Pocket hotbar panel height
   - Lines 258, 282, 308: Hotbar offset adjustments (increase if hotbar is larger)

4. **Offset adjustments** / **Offset-Anpassungen:**
   - If hotbar appears too high/low, adjust "offset" values in lines 258, 282, 308
   - Increase the second number (e.g., from 16 to 24) if hotbar is larger
   - Wenn die Hotbar zu hoch/niedrig erscheint, passen Sie die "offset"-Werte an

---

## UUID Information / UUID-Informationen

**Do NOT change these unless creating a new pack / NICHT ändern, es sei denn, Sie erstellen ein neues Pack:**

- Header UUID: `4b84ef0b-9a8f-40fb-b07a-82a7fa8a13a5`
- Module UUID: `d6d2daaa-2b90-42c6-ac72-17a16a533ad5`

These UUIDs are unique to this pack and ensure it doesn't conflict with others.
Diese UUIDs sind einzigartig für dieses Pack und stellen sicher, dass es nicht mit anderen kollidiert.
