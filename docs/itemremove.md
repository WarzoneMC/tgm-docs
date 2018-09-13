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

To resolve material names, please use the [Spigot Javadocs](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html). Do not use IDs for items (as they are deprecated), and do not use legacy material names (such as `LEGACY_DEAD_BUSH`). It is recommended to keep material names in lowercase and use spaces instead of underscores for readability.
