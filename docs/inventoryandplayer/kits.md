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
				{"type": "item", "material": "oak planks", "slot": 1, "amount": 64},

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
                {"material": "red stained glass", "slot": 4, "amount": 64}
            ]
        },
        {
            "name": "blue_kit",
            "teams": ["blue"],
            "items": [
                {"material": "blue stained glass", "slot": 4, "amount": 64}
            ]
        }
    ]
```

### Kit Attributes

| Attribute     | Description                                                   | Value   |
|---------------|---------------------------------------------------------------|---------|
| `name`        | The name of the kit.                                          | String  |
| `teams`       | The teams that receive the kit (separated by a comma)         | String  |
| `items`       | Contains child attributes such as the material and amount.    | Parent  |
| `effects`     | Contains child attributes such as effect and duration.        | Parent  |

### Items Attributes

| Attribute     | Description                                                   | Value   |
|---------------|---------------------------------------------------------------|---------|
| `type`        | The type of material the player will be receiving             | String  |
| `material`    | The item or armor the player will be receiving                | String  |
| `slot`        | The slot the item will spawn in.                              | Slot    |
| `amount`      | The amount of an item the player receives. Default is 1.      | Number  |
| `unbreakable` | Whether the item is breakable or not.                         | Boolean |
| `displayName` | The name of the item.                                         | String  |
| `lore`        | The subtext (lore) of the item.                               | String  |
| `flags`       | The type of flags that are applied to the item.               | Parent  |

#### Flags Attributes

| Attribute        | Description                                                   | Value   |
|------------------|---------------------------------------------------------------|---------|
| `hide_attributes`| Hides attributes like damage.                                 | Boolean |
| `hide_destroys`  | Hides what an item stack can destroy.                         | Boolean |
| `hide_enchants`  | Hides what enchantments the item has.                         | Boolean |
| `hide_placed_on` |  Hides what a block can be placed against.                    | Boolean |
| `hide_potion_effects`|  Hides the potion effects on an item stack.               | Boolean |
| `hide_unbreakable` |  Hides the unbreakable state.                               | Boolean |


### Effects Attributes

| Attribute     | Description                                                   | Value   |
|---------------|---------------------------------------------------------------|---------|
| `effect`      | The type of effect the player will be receiving               | String  |
| `duration`    | The duration of time that the player will recieve this effect | Number  |
| `amplifier`   | The "level" (or strength) of the effect                       | Number  |
| `particles`   | Whether or not particles will display during the effect       | Boolean |
| `ambient`     | Makes potion effect produce more, translucent, particles      | Boolean |

<span class="label label-note">Note</span> You can additionally assign more than 1 kit to a team as long as the slots don't overlap.
