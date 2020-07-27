# Killstreaks

This module is used to perform actions via automated commands, activated when a player obtains a kill. This module can give potion effects, teleport them to a location, play a sound, change the weather, or even modify the gamerule.

## Example

Get an golden apple for every kill.

```json
    "killstreaks": [
        {
            "count": 1,
            "repeat": true,
            "actions": {
                "items": [
                    {"material": "golden apple", "amount": 1}
                ]
            }
        }
    ]
```

Give the player regeneration for every kill.

```json
    "killstreaks": [
        {
            "count": 1,
            "repeat": true,
            "actions": {
                "effects": [
                    {"type": "regeneration", "duration": 2}
                ]
            }
        }
    ]
```

Shoot a firework everytime the player hits a 5 kill streak.

```json
    "killstreaks": [
        {
            "count": 5,
            "repeat": true,
            "actions": {
                "fireworks": [
                    {"type": "creeper", "trail": true, "flicker": true, "colors": [16753920], "fade_colors": [16753920], "lifetime": 0}
                ]
            }
        }
    ]
```

When a player reaches 10 kills, clear all of the villagers in the map.

```json
    "killstreaks": [
        {
            "count": 10,
            "repeat": false,
            "commands": [
                "kill @e[type=!Villager]"
            ]
        }
    ]
```

### Killstreak Attributes

| Attribute | Description                                                           | Value   |
|-----------|-----------------------------------------------------------------------|---------|
| `count`   | The amount of kills required before the command is executed.          | Number  |
| `repeat`  | Whether or not the command should activate each time.                 | Boolean |
| `actions` | The item, potion effect, or sound effect that should be executed.     | String  |
| `commands`| The command that should be executed.                                  | Command |

### Action Attributes

| Attribute   | Description                                                           | Value     |
|-------------|-----------------------------------------------------------------------|-----------|
| `items`     | The item that should be given to the player.                          | Item      |
| `effects`   | Potion effect that's given to the player.                             | Effect    |
| `fireworks` | The type of firework that should be shot off at the player.           | Firework  |
| `sounds`    | Sound effect that should be played.                                   | Sound     |

### Firework Attributes

| Attribute        | Description                                                           | Value     |
|------------------|-----------------------------------------------------------------------|-----------|
| `type`           | The type of firework launched (design).                               | String    |
| `trail`          | If the firework should have a trail or not.                           | Boolean   |
| `flicker`        | Whether the firework will flicker or not.                             | Boolean   |
| `colors`         | The colors of the initial firework launched.                          | Color     |
| `fade_colors`    | The colors of the firework as it fades away.                          | Color     |
| `lifetime`       | The length the firework should appear in the air.                     | Number    |

### Sound Attributes

By default, certain killstreaks amounts already play sound effects without inserting anything.

| Attribute   | Description                                                           | Value     |
|-------------|-----------------------------------------------------------------------|-----------|
| `sound`     | Sound effect that will be played.                                     | Sound     |
| `volume`    | The volume of the sound effect being played.                          | Number    |
| `pitch`     | Pitch of the sound effect being played.                               | Number    |
| `target`    | Who hears the sound, default is everyone. "player" or "everyone"      | String    |

<span class="label label-note">Note</span> Malicious commands are punishable.
