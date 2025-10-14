# INSTALLATION GUIDE / INSTALLATIONSANLEITUNG

## English

### Quick Installation
1. Copy the entire `custom_hotbar_pack` folder to your Minecraft resource packs directory:
   - **Windows 10/11**: `%localappdata%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs\`
   - **Android**: `sdcard/games/com.mojang/resource_packs/`
   - **iOS**: `On My iPhone/Minecraft/games/com.mojang/resource_packs/`
   - **Dedicated Server**: `<server_directory>/resource_packs/`

2. Launch Minecraft Bedrock Edition
3. Go to Settings → Global Resources
4. Find "Custom Hotbar Size" in the available packs
5. Click to activate it
6. The hotbar will now be 150% larger (adjustable)

### Customizing the Hotbar Size

Edit `ui/hud_screen.json` to change the size:

**For Desktop/PC** (line 7):
```json
"$hotbar_renderer_size|default": [ 30, 33 ],
```
Change `[ 30, 33 ]` to your preferred size.

**For Mobile/Pocket** (line 73):
```json
"size": [ "100%", 60 ],
```
Change `60` to your preferred height.

### Recommended Sizes

**Desktop (Default 20x22):**
- Small (75%): `[ 15, 16.5 ]`
- Normal (100%): `[ 20, 22 ]`
- Large (125%): `[ 25, 27.5 ]`
- Very Large (150%): `[ 30, 33 ]` ← Current setting
- Huge (200%): `[ 40, 44 ]`

**Pocket (Default 40):**
- Small (75%): `30`
- Normal (100%): `40`
- Large (125%): `50`
- Very Large (150%): `60` ← Current setting
- Huge (200%): `80`

---

## Deutsch

### Schnellinstallation
1. Kopieren Sie den gesamten Ordner `custom_hotbar_pack` in Ihr Minecraft-Ressourcenpakete-Verzeichnis:
   - **Windows 10/11**: `%localappdata%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs\`
   - **Android**: `sdcard/games/com.mojang/resource_packs/`
   - **iOS**: `On My iPhone/Minecraft/games/com.mojang/resource_packs/`
   - **Dedizierter Server**: `<server_verzeichnis>/resource_packs/`

2. Starten Sie Minecraft Bedrock Edition
3. Gehen Sie zu Einstellungen → Globale Ressourcen
4. Finden Sie "Custom Hotbar Size" in den verfügbaren Paketen
5. Klicken Sie zum Aktivieren
6. Die Hotbar ist jetzt 150% größer (anpassbar)

### Anpassung der Hotbar-Größe

Bearbeiten Sie `ui/hud_screen.json`, um die Größe zu ändern:

**Für Desktop/PC** (Zeile 7):
```json
"$hotbar_renderer_size|default": [ 30, 33 ],
```
Ändern Sie `[ 30, 33 ]` zu Ihrer bevorzugten Größe.

**Für Mobile/Pocket** (Zeile 73):
```json
"size": [ "100%", 60 ],
```
Ändern Sie `60` zu Ihrer bevorzugten Höhe.

### Empfohlene Größen

**Desktop (Standard 20x22):**
- Klein (75%): `[ 15, 16.5 ]`
- Normal (100%): `[ 20, 22 ]`
- Groß (125%): `[ 25, 27.5 ]`
- Sehr groß (150%): `[ 30, 33 ]` ← Aktuelle Einstellung
- Riesig (200%): `[ 40, 44 ]`

**Pocket (Standard 40):**
- Klein (75%): `30`
- Normal (100%): `40`
- Groß (125%): `50`
- Sehr groß (150%): `60` ← Aktuelle Einstellung
- Riesig (200%): `80`

---

## Technical Notes / Technische Hinweise

- The pack uses unique UUIDs to avoid conflicts / Das Pack verwendet eindeutige UUIDs, um Konflikte zu vermeiden
- Compatible with Minecraft Bedrock 1.21.0+ / Kompatibel mit Minecraft Bedrock 1.21.0+
- Changes are visual only and don't affect gameplay / Änderungen sind nur visuell und beeinflussen nicht das Gameplay
- You can adjust the offset values if the hotbar position needs tweaking / Sie können die Offset-Werte anpassen, wenn die Hotbar-Position angepasst werden muss
