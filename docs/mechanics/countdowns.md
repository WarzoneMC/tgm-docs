# Countdowns

This module is used to create custom countdowns on the server.

## Example

Run a custom countdown that says "dinosaurs" and triggers test1

```JSON
	"countdowns": [
		{
			"id": "test",
			"title": "Countdown 1: %countdownTimeLeft%",
			"time": 5,
			"color": "purple",
			"style": "solid",
			"visible": true,
			"invert": false,
			"teams": ["red", "blue"],
			"onFinish": [
				"say yeet",
				"countdown start test1"
			]
		},
		{
			"id": "test1",
			"title": "Countdown 2: %countdownTimeLeft%",
			"time": 5,
			"color": "green",
			"style": "segmented 12",
			"visible": true,
			"invert": true,
			"teams": ["red", "blue"],
			"onFinish": [
				"say yote",
				"countdown start test"
			]
		}
	],
```

### Countdown Structure
Field | Description | Type | Required | Default
--- | --- | --- | --- | ---
`id` | ID of the countdown used to start, edit or cancel it. | String | Yes |
`time` | Duration of the countdown in **seconds**. | Integer | Yes |
`title` | Text displayed on the boss bar. | String | Yes |
`color` | Color for boss bar. (`BLUE`, `GREEN`, `PINK`, `PURPLE`, `RED`, `WHITE`, `YELLOW`) | String | No | `PURPLE`
`style` | Style for the boss bar. (`SOLID`, `SEGMENTED_6`, `SEGMENTED_10`, `SEGMENTED_12`, `SEGMENTED_20`) | String | No | `SOLID`
`visible` | Make the boss bar visible. | Boolean | No | `true`
`invert` | Make the boss bar go in the opposite direction. | Boolean | No | `false`
`teams` | Teams that are able to see the boss bar. | String array | No | All teams
`onFinish` | Commands that will run when the countdown ends. | String array | No |
