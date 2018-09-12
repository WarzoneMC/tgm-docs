# Portals

This module is used to teleport players to different parts of the map.

## Example

```json
    "portals": [ 
        {"from": "blue-portal", "to": "10, 23, 34, 180", "teams": ["blue"], "sound": false}
    ],
```

### Portal Attributes

| Attribute | Description                                                         | Value      |
|-----------|---------------------------------------------------------------------|------------|
| `from`    | The location in which the player must enter from.                   | Region     |
| `to`      | The location in which the player is teleported to.                  | Coordinate |
| `teams`   | The teams that are allowed to enter through this portal.            | String     |
| `sound`   | Whether or not the default "zip" sound should be played upon entry. | String     |

**NOTE:** A region is required to define `from`. Portals are also automatically enabled for spectators.
