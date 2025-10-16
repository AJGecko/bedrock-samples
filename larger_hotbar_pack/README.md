# Größere Hotbar Ressourcenpack für Minecraft Bedrock Edition (Mobile)

🎮 **Komplett fertig und sofort einsetzbar!**

Dieses Ressourcenpack macht die Hotbar und alle HUD-Elemente auf dem Handy größer für bessere Sichtbarkeit und einfachere Bedienung.

> **Hinweis:** Dieses Pack ist vollständig konfiguriert und kann direkt in Minecraft verwendet werden. Einfach den Ordner kopieren und installieren!

## Funktionen

- **Vergrößerte Hotbar**: Die Hotbar ist um 50% größer (von 20x22 auf 30x33 Pixel pro Slot)
- **Vergrößerte Herzen**: Lebensanzeige ist 50% größer für bessere Sichtbarkeit
- **Vergrößerte Hunger-Bar**: Hungeranzeige ist 50% größer
- **Vergrößerte Rüstungsanzeige**: Rüstungspunkte sind 50% größer
- **Vergrößerte XP-Bar**: Erfahrungsleiste ist 50% größer
- **Vergrößerte Luft-Blasen**: Sauerstoffanzeige ist 50% größer
- **Alle Buttons bleiben funktionsfähig**: Inventarknopf, Elipsen-Buttons und alle anderen UI-Elemente funktionieren weiterhin
- **Korrekte Hitboxen**: Alle Inventar-Slots und Buttons haben die richtigen Hitboxen

## Installation

### Für Android/iOS:

1. Kopiere den Ordner `larger_hotbar_pack` auf dein Gerät
2. Verschiebe den Ordner nach:
   - **Android**: `Android/data/com.mojang.minecraftpe/files/games/com.mojang/resource_packs/`
   - **iOS**: `Minecraft PE/games/com.mojang/resource_packs/`
3. Starte Minecraft Bedrock Edition
4. Gehe zu Einstellungen → Globale Ressourcen
5. Aktiviere "Größere Hotbar Pack"
6. Fertig! Die Änderungen werden sofort angewendet

### Alternative Installation (Dateimanager):

1. Benenne den Ordner `larger_hotbar_pack` zu `larger_hotbar_pack.mcpack` um
2. Tippe auf die .mcpack Datei
3. Minecraft öffnet sich automatisch und importiert das Pack
4. Aktiviere es in den globalen Ressourcen

## Kompatibilität

- **Minecraft Bedrock Edition**: Version 1.21.0 oder höher
- **Plattformen**: Android, iOS, Windows 10/11, Xbox, PlayStation, Nintendo Switch
- **Optimiert für**: Mobile Geräte (Handy/Tablet)

## Technische Details

Das Pack modifiziert folgende Elemente:

- **Hotbar Renderer**: Vergrößerte Slot-Größe (30x33px)
- **Heart Renderer**: 1.5x Skalierung
- **Hunger Renderer**: 1.5x Skalierung
- **Armor Renderer**: 1.5x Skalierung
- **Bubble Renderer**: 1.5x Skalierung
- **XP Bar**: 1.5x Höhe (7.5px statt 5px)
- **Hotbar Panel (Pocket)**: Vergrößert auf 60px Höhe

## Hinweise

- Das Pack funktioniert mit allen anderen Packs, die nicht die gleichen UI-Elemente modifizieren
- Bei Konflikten mit anderen UI-Packs, stelle sicher dass dieses Pack höher in der Liste steht
- Die Standard-Texturen werden verwendet, nur die Größen werden angepasst

## Problemlösung

**Problem**: Die UI-Elemente sind zu groß
- **Lösung**: Die Skalierungsfaktoren können in der Datei `ui/hud_screen.json` angepasst werden

**Problem**: Buttons funktionieren nicht
- **Lösung**: Stelle sicher, dass das Pack korrekt installiert ist und keine anderen UI-Packs Konflikte verursachen

**Problem**: Pack wird nicht erkannt
- **Lösung**: Überprüfe, ob die `manifest.json` vorhanden ist und das Pack im richtigen Ordner liegt

## Credits

Erstellt für bessere Spielbarkeit auf mobilen Geräten.
Basiert auf den Vanilla Bedrock Samples.

## Lizenz

Dieses Pack ist frei verwendbar für private Zwecke.
