# Killstreaks

This module is used to perform actions via automated commands, activated when a player obtains a kill. This module can give potion effects, teleport them to a location, play a sound, change the weather, or even modify the gamerule. All commands are executed by the console.

## Example

Get an arrow for every kill.

```json
    "killstreaks": [
        {"count": 1, "repeat": true, "commands":["give %killername% arrow 1"]}
    ],
```

When a player reaches 10 kills, clear all of the villagers in the map.

```json
    "killstreaks": [
        {"count": 10, "repeat": false, "commands":["kill @e[type=!Villager]"]}
    ],
```

### Killstreak Attributes

| Attribute | Description                                                           | Value  |
|-----------|-----------------------------------------------------------------------|--------|
| `count`   | The amount of kills required before the command is executed.          | Number |
| `repeat`  | Whether or not the command should activate each time.                 | Boolean|
| `commands`| The command that should be executed.                                  | Command|

**NOTE:** Malicious commands are punishable.
