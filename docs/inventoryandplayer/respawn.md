# Respawn

This module is used to modify player respawning.

## Example

```json
	"respawn": {
		"rules": [
			{
				"freeze": true,
				"blindness": true,
				"confirm": false,
				"delay": 4000
			}
		]
	},
```

### Respawn Attributes

| Attribute | Description                                                           | Value    | Default |
|-----------|-----------------------------------------------------------------------|----------|---------|
| `rules`   | The attribute which fosters the mechanics that are modified. | Parent    |      |


### Rules Attributes

| Attribute | Description                                                           | Value    | Default |
|-----------|-----------------------------------------------------------------------|----------|---------|
| `delay`   | The duration until the player is allowed to respawn. | Value    |      |
| `freeze`   | Whether or not the player may move when in the death screen. | Boolean     |      |
| `blindness`  | Whether or not the player can see when in the death screen.  | Boolean     |           |
| `confirm`  | Whether or not the player must interact with the death screen to respawn.  | Boolean     |           |
| `teams`  | Defines which teams will be affected by rules attributes.  | Team ID     |           |
