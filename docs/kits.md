# Kits & Inventory

This module is used to define the default kit each player recieves in their inventory during the match. The kits are given to each player at the start of each match and whenever they respawn.

## Example

Gives all players an iron sword and wood as well as armor.

```json
    "kits": [
		{
			"name": "Default",
			"items": [
				{"type": "item", "material": "iron sword", "slot": 0},
				{"type": "item", "material": "wood", "slot": 1, "amount": 64},

				{"material": "leather helmet", "slot": "helmet", "unbreakable": true},
				{"material": "iron chestplate", "slot": "chestplate", "unbreakable": true},
				{"material": "leather leggings", "slot": "leggings", "unbreakable": true},
				{"material": "chainmail boots", "slot": "boots", "unbreakable": true}
			]
		}
	]
```
Defines which kit each team receives.

```json
    "kits": [
        {
            "name": "red_kit",
            "teams": ["red"],
            "items": [
                {"material": "stained glass", "slot": 4, "amount": 64, "durability": 14}
            ]
        },
        {
            "name": "blue_kit",
            "teams": ["blue"],
            "items": [
                {"material": "stained glass", "slot": 4, "amount": 64, "durability": 11}
            ]
        }
    ]
```

### Team Attributes

| Attribute     | Description                                                   | Value   |
|---------------|---------------------------------------------------------------|---------|
| `type`        | The type of material the player will be receiving             | String  |
| `material`    | The item or armor the player will be receiving                | String  |
| `slot`        | The slot the item will spawn in.                              | Slot    |
| `amount`      | The amount of an item the player receives. Default is 1.      | Number  |
| `durability`  | The certain ID of the block the player receives.              | Number  |
| `unbreakable` | Whether the item is breakable or not.                         | Boolean |

<span class="label label-note">Note</span> You can additionally assign more than 1 kit to a team as long as the slots don't overlap.
