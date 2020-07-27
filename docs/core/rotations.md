# Rotations
As of July 5th 2020 Warzone no longer uses rotation.txt and now uses rotation.json to utilise multiple (dynamic) rotations. Rotations now have support to add multiple rotations, each rotation having its own name and 'requirements' such as the number of players needed.

If a rotation is manually set by a user that has permissions, the rotation should start from the beginning and then play through to the end and once the rotation has been completed it should automatically return to the normal or "default" rotation.

## Commands
A few commands were added to update and change the current active rotation.
### rotation
View all of the maps in the current rotation.<br>
**Alias:** rot<br>
**Usage:** `rotation [page]`
<hr>

### rotations
View all of the rotations currently in the repository.<br>
**Alias:** rots<br>
**Usage:** `rotations`
<hr>

### setrotation
Sets the current rotation.<br>
**Permission Node:** `tgm.command.setrot`<br>
**Alias:** setrot<br>
**Usage:** `setrotation [rotation]`<br>
<span class="label label-note">Note</span> Use /rotations to view the avaliable options.
<hr>

## Dynamic Rotation Example
```json
[
	{
		"name": "smol",
		"default": true,
		"requirements": {
			"min": 0,
			"max": 10
		},
		"maps": [
			"map1",
			"map2",
			"map3",
			"map4"
		]
	},
	{
		"name": "big",
		"default": true,
		"requirements": {
			"min": 11,
			"max": 30
		},
		"maps": [
			"map1",
			"map2",
			"map3",
			"map4"
		]
	},
	{
		"name": "infected",
		"maps": [
			"map1",
			"map2",
			"map3",
			"map4"
		]
	}
]
```

>#### name
Name of the rotation.

>#### default
Whether this rotation is the default rotation.

>#### requirements
**min**: Minimum amount of people for this rotation to be used.<br>
**max**: Maximum amount of people for this rotation to be used.

>#### maps
List of maps in the rotation.
