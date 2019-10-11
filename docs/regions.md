# Regions

This module is used to specify the bounds in which a filter is used.

## Example

```json
	"regions": [
		{ "id": "cub-region", "type": "cuboid", "min": "-94, 16, -4", "max": "-103, 23, 4" },
		{ "id": "cyl-region", "type": "cylinder", "base": "-79, 7, -2", "radius": 3, "height": 6 },
		{ "id": "sph-region", "type": "sphere", "center": "-35, 83, 22", "radius": 5 },
		{ "id": "hsp-region", "type": "hemisphere", "center": "-26, 48, 24", "radius": 8, "direction": "-x"},
		{ "id": "mta-region", "type": "meta", "regions": ["blue-spawn-protection", "red-spawn-protection"]}
	],
```

### Spawn Attributes

| Attribute | Description                                                                                       | Value    |
|-----------|---------------------------------------------------------------------------------------------------|----------|
| `id`      | The unique ID that you are naming the region. Used later for filters.                             | ID       |
| `type`    | The type of geometry that the region uses (`cuboid`, `cylinder`, `sphere`, `hemisphere`, `meta`)  | String   |

---

#### Cuboid Attributes

| Attribute | Description                                                           | Value    |
|-----------|-----------------------------------------------------------------------|----------|
| `min`     | The first corner of the cuboid, as an `XYZ` value.                    | Coords   |
| `max`     | The second corner of the cuboid, as an `XYZ` value.                   | Coords   |

#### Cylinder Attributes

| Attribute | Description                                                           | Value    |
|-----------|-----------------------------------------------------------------------|----------|
| `base`    | The center block of the cylinder, as an `XYZ` value.                  | Coords   |
| `radius`  | How many blocks outward the cylinder region extends.                  | Number   |
| `height`  | How many blocks high the cylinder region extends.                     | Number   |

#### Sphere Attributes

| Attribute | Description                                                           | Value    |
|-----------|-----------------------------------------------------------------------|----------|
| `center`  | The center block of the sphere, as an `XYZ` value.                    | Coords   |
| `radius`  | How many blocks outward the sphere region extends.                    | Number   |

#### Hemisphere Attributes

| Attribute | Description                                                           | Value    |
|-----------|-----------------------------------------------------------------------|----------|
| `center`  | The center block of the hemisphere, as an `XYZ` value.                | Coords   |
| `radius`  | How many blocks outward the hemisphere region extends.                | Number   |
| `direction`| Which direction the hemisphere is facing (`+/- x,y,z`)               | Direction|

#### Meta Attributes

| Attribute | Description                                                           | Value    |
|-----------|-----------------------------------------------------------------------|----------|
| `regions` | References several regions/coordinates.                               | Coords / Region ID   |

<span class="label label-note">Note</span> More region types will be supported in the future.
