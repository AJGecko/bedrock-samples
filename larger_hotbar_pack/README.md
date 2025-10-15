# Larger Hotbar Resource Pack

This resource pack makes the hotbar in Minecraft Bedrock Edition larger for better visibility.

## Features

- **Larger Hotbar Slots**: The hotbar slots are increased from 20x22 pixels to 30x33 pixels (50% larger)
- **Larger Item Icons**: Item icons are scaled up from 16x16 to 24x24 pixels
- **Larger Selected Slot Indicator**: The selected slot frame is increased from 24x24 to 36x36 pixels
- **Proper Container Sizing**: The exp_progress_bar_and_hotbar container is resized to 42 pixels height to accommodate the larger hotbar
- **All Elements Scaled Proportionally**: Includes caps, buttons, and other UI elements
- **Classic UI Compatible**: Fixes alignment and centering issues with the Classic UI

## Installation

1. Copy the entire `larger_hotbar_pack` folder to your Minecraft resource packs folder:
   - **Windows**: `%localappdata%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs\`
   - **Android**: `/storage/emulated/0/games/com.mojang/resource_packs/`
   - **iOS**: `Apps/com.mojang.minecraftpe/Documents/games/com.mojang/resource_packs/`

2. Open Minecraft Bedrock Edition

3. Go to **Settings** > **Global Resources**

4. Find "Larger Hotbar Resource Pack" in the available packs list

5. Click the **+** button to activate it

6. Click **Apply** or restart the game if needed

## Customization

To adjust the hotbar size, edit the `ui/hud_screen.json` file and modify the size values:

- **Default size**: `[ 20, 22 ]` (width, height in pixels)
- **Current size**: `[ 30, 33 ]` (50% larger)

You can change these values to any size you prefer. For example:
- **75% larger**: `[ 35, 38.5 ]`
- **100% larger**: `[ 40, 44 ]`
- **25% larger**: `[ 25, 27.5 ]`

**Important**: When changing the hotbar size, make sure to update:
1. All hotbar element sizes in the file (hotbar_renderer_size, gui_hotbar_grid_item, etc.)
2. The `exp_progress_bar_and_hotbar` container height: Calculate as `5 (XP bar) + 16 (offset) + hotbar_height + 5 (padding)`
   - For 50% larger (33px hotbar): `42` pixels
   - For 100% larger (44px hotbar): `53` pixels
   - For 25% larger (27.5px hotbar): `36.5` pixels

## Technical Details

**Format Version**: 2  
**Minimum Engine Version**: 1.21.0

**UUIDs**:
- Header: `6423d417-3bfa-4f02-9261-a4503fa8049d`
- Module: `5b355b56-eee8-46f9-808b-3bb398b599d9`

These UUIDs are unique to this resource pack and ensure it doesn't conflict with other packs.

## Compatibility

- Works with Minecraft Bedrock Edition version 1.21.0 and later
- Compatible with other resource packs (load order may matter)
- Should work on all platforms (Windows, Android, iOS, Xbox, PlayStation, Nintendo Switch)

## Troubleshooting

**Hotbar not changing size:**
- Make sure the resource pack is activated in Settings > Global Resources
- Try restarting Minecraft
- Check that no other resource pack is overriding the hotbar UI

**UI elements misaligned:**
- This is expected if using with certain custom UIs
- Adjust the resource pack load order in the Global Resources menu

## License

This resource pack is provided as-is for use with Minecraft Bedrock Edition. You may modify and redistribute it freely.
