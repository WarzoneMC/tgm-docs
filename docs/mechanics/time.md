# Time

This module is used to modify certain facets of how a winner is determined using time limits and set broadcasts.

## Example

- Sets the time limit to 20 minutes (1200 seconds)
- When the time limit is up, blue wins by default
- Every 10 seconds, a "Test" will be broadcasted and the `give @a arrow 1` command will be ran

```JSON
	"time": {
		"limit": 1200,
		"defaultWinner": "blue",
		"broadcasts": [
			{
				"message": "Test",
				"interval": 10,
				"repeat": true,
				"commands": [
					"give @a arrow 1"
				]
			}
		]
	},
```

`limit` and `interval` is in seconds.
