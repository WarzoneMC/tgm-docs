# Item Removal

This module is used to remove certain items when they are dropped.

## Example

Disable inventory drops and obsidian.

```json
	"itemremove": [
		"iron sword", "bow", "diamond pickaxe", "iron axe", "glass",
		"cooked beef", "arrow", "leather helmet", "chainmail chestplate",
		"leather leggings", "leather boots", "obsidian"
	],
```
Disable item drops specifically on death, manual removal, and spawn (such as breaking blocks).

```json
	"itemremove": [
		{
			"type": "red wool",
			"death": true,
			"drop": true,
			"spawn": true
		}
	],
```
To disable all inventory drops:

```json
       "itemremove": "*",
```

To resolve material names, please use the [Spigot Javadocs](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html). Do not use IDs for items (as they are deprecated), and do not use legacy material names (such as `LEGACY_DEAD_BUSH`). It is recommended to keep material names in lowercase and use spaces instead of underscores for readability.
