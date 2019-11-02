# Generators

This module is used to generate items in a map, with various tiers.

## Example

```json
  "generators": [
    {
      "id": "middle-generator",
      "item": {
        "material": "diamond"
      },
      "location": "77, 6, 27",
      "limit": 4,
      "range": 5,
      "interval": 1200,
      "hologram": {
        "timeUnit": "seconds",
        "content": "&bDiamond &ewill spawn in &c%time% &e%span%"
      },
      "upgrades": {
        "type": "scheduled",
        "sequence": [
          {
            "time": 600,
            "interval": 600,
            "message": "&eGenerator &7has been upgraded to &eLevel %level%!",
            "item": {
              "material": "emerald"
            },
            "holoContent": "&aEmerald &ewill spawn in &c%time% &6%span%"
          }
        ]
      }
    }
  ]
}
```

### Generators Attributes

| Attribute     | Description                                              | Value      |
|---------------|----------------------------------------------------------|------------|
| `id`        | The name of the generator.       | String    |
| `item`        | 	Nests the material and other item attributes.       | Item    |
| `location` | The coordinates in which the item will spawn.   | Coordinate    |
| `limit`        | The amount of items active in a stack at a given time.      | Number    |
| `range`        | 		The distance a player must be within range (in blocks) for spawning.       | Number    |
| `interval` | The frequency of the item spawn.   | Number   |
| `hologram`        | 	The hologram that may display information about the generator.       | Parent    |
| `upgrades`        | 	The parent attribute that stores generator "tier" upgrading.       | Parent    |

### Hologram Attributes

| Attribute     | Description                                              | Value      |
|---------------|----------------------------------------------------------|------------|
| `timeUnit`        | 	The unit of time measurement used.       | Boolean    |
| `content` | 	The display of the hologram (in text - colors may be used with `&`.)   | Boolean    |

### Upgrades Attributes

| Attribute     | Description                                              | Value      |
|---------------|----------------------------------------------------------|------------|
| `no`        | 	someone else do this section       | idiot    |
