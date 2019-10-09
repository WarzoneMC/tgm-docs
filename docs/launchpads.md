# Launchpads

This module is used to specify where players will appear when they first join the match. This is typically at the team's base, in a protected region.

## Example

```json
	"launchpads": [
		{
			"region": {"type": "cuboid", "min": "9, 29, -124", "max": "9, 29, -124"},
			"delay": 2,
			"motion": "-0.35, 2.25, 0.35",
			"directional": false,
			"teams": ["blue"]
		},
		{
			"region": "blue-launchpad",
			"delay": 2,
			"motion": "-0.35, 2.25, 0.35",
			"directional": false,
			"teams": ["blue"]
		}
	],
```

### Spawn Attributes

Field name | Description | Type | Required
--- | --- | --- | ---
`region` | Area where the player needs to stand to be launched. | Region ID or [Region Object](https://docs.warz.one/#/regions) | **Yes**
`delay` | How long in ticks the player needs to stand to be launched. | Integer | No (Default: 0)
`directional` | Whether the launchpad should launch the player in the direction they are looking at. | Boolean | No (Default: true)
`motion` | Direction in which the player will be launched. If the `directional` field is set to **true**, this will act as a multiplier for the player's direction. | Vector (x, y ,z) | No (Default: 1, 1, 1)
`teams` | List of teams that can use the launch pad. | List of teams | No (Default: all teams)
