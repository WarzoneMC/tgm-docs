# Filters

This module is used to apply conditions to players, blocks, and events. This is used in conjunction with regions to determine exactly what should happen to certain things in the match, by declaring `DENY`, `ALLOW`, or `ABSTAIN`. Filters are the most useful feature to customize your maps and make them unique.

## Example

Prevent explosions from destroying the `blue-spawn` region.

```json
	"filters": [
		{
			"type": "block-explode", "evaluate": "deny", "teams": ["blue", "red"],
			"regions": ["blue-spawn"], "message": "&cYou are not allowed to modify terrain here."
		}
	],
	"regions": [
		{"id": "blue-spawn", "type": "cuboid", "min": "121, 16, -33", "max": "123, 12, -35"}
	]
```

Prevent players from building out the `map` region.

```json
	"filters": [
		{
			"type": "build", "evaluate": "deny", "inverted": true, "teams": ["blue", "red"],
			"regions": ["map"], "message": "&cYou cannot build outside of the map."
		}
	],
	"regions": [
		{"id": "map", "type": "cuboid", "min": "-46, 0, -184", "max": "46, oo, 328"}
	]
```

### Filter Attributes

| Attribute | Description                                                           | Value   |
|-----------|-----------------------------------------------------------------------|---------|
| `type`    | The **type** of filter used to apply a condition.                     | String  |
| `evaluate`| How the condition applies to the team (`DENY`, `ALLOW`, `ABSTAIN`)    | String  |
| `inverted`| If the filter is inverted (applies everywhere the region doesn't)     | Boolean |
| `teams`   | The teams that the filter applies to.                                 | Team    |
| `message` | The message that should be sent to players when the filter activates. | String  |
| `regions` | The regions that the filter is meant to modify.                       | Region  |

The types of filters allowed to be used are filters that are coded into TGM: Therefore, you cannot modify events that are not already supported. The types of filters are listed below, used in conjunction with `type`.

### Type Attributes

| Attribute      | Description                                                                 | Value  |
|----------------|-----------------------------------------------------------------------------|--------|
| `build`           | Determines whether or not players can interact with the region.          | String |
| `enter`           | Determines whether or not players can enter a specified region.          | String |
| `leave`           | Determines whether or not players can leave/exit a specified region.     | String |
| `renewable-blocks`| Determines how blocks are regenerated after being mined.                 | String |
| `block-explode`   | Determines whether or not explosions destroy a specified region.         | String |
| `block-interact`  | Determines whether or not players can interact with a region.            | String |
| `block-place`     | Determines whether or not players can place blocks.                      | String |
| `block-break`     | Determines whether or not players can break blocks.                      | String |
| `void-build`      | Determines how blocks in a specified void region can be interacted with. | String |
| `use-bow`         | Determines whether or not players should be allowed to fire arrows.      | String |
| `use-shear`       | Determines whether or not players should be allowed to shear sheep.      | String |

<span class="label label-note">Note</span> More filters are planned to be added in the future.
