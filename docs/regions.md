# Regions

This module is used to specify the bounds in which a filter is used. TGM currently supports `CUBOID` (min, max) & `CYLINDER` (base, radius, height) regions.

## Example

```json
	"regions": [
		{ "id": "l-spawn", "type": "cuboid", "min": "-94, 16, -4", "max": "-103, 23, 4" },
		{ "id": "r-spawn", "type": "cuboid", "min": "56, 16, 4", "max": "64, 23, -4" },
		{ "id": "s-spawn", "type": "cylinder", "base": "-79, 7, -2", "radius": "3", "height": "6" }
	],
```

### Spawn Attributes

| Attribute | Description                                                           | Value    |
|-----------|-----------------------------------------------------------------------|----------|
| `id`      | The unique ID that you are naming the region. Used later for filters. | ID       |
| `type`    | The type of geometry that the region uses (`cuboid`, `cylinder`)      | String   |

---

#### Cuboid Attributes

| Attribute | Description                                                           | Value    |
|-----------|-----------------------------------------------------------------------|----------|
| `min`     | The first corner of your cuboid, as an `XYZ` value.                   | Coords   |
| `max`     | The second corner of your cuboid, as an `XYZ` value.                  | Coords   |

#### Cylinder Attributes

| Attribute | Description                                                           | Value    |
|-----------|-----------------------------------------------------------------------|----------|
| `base`    | The center block of your cylinder, as an `XYZ` value.                 | Coords   |
| `radius`  | How many blocks outward the cylinder region extends.                  | Number   |
| `height`  | How many blocks high the cylinder region extends.                     | Number   |

**NOTE:** More region types, such as sphere and void, will be supported in the future.
