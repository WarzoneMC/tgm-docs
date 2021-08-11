# Spawns

This module is used to specify where players will appear when they first join the match. This is typically at the team's base, in a protected region.

## Example

```json
	"spawns": [
		{"teams": ["spectators"], "coords": "0.5, 63, 0.5, -180"},
		{"teams": ["red"], "coords": "23.5, 9, 27.5, 90"},
		{"teams": ["blue"], "coords": "-22.5, 9, -26.5, -90"}
	],
```

### Spawn Attributes

| Attribute | Description                                                                    | Value    |
|-----------|--------------------------------------------------------------------------------|----------|
| `teams`           | The name of the teams that spawn at the coords. Must use the Team ID.  | Team     |
| `coords`          | The coordinates at which the team spawns.                              | Location |
| `yaw`             | The yaw of which a player faces upon spawning.                         | Value    |
| `pitch`           | The pitch of which a player faces upon spawning.                       | Value    |
| `face-coordinates`| A point which spawns all players to face towards its direction.        | Location |
| `region`          | A region in which players spawn into (can be used to randomize spawns) | Region |

<span class="label label-note">Note</span> `coords` requires the X, Y, Z, and YAW (in that order). Coordinates can be seen by pressing F3.
