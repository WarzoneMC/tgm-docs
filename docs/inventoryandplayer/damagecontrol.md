# Damage Control

This module is used to determine whether or not damage is taken as a result of various player actions.

## Example

```json
"damageControl": {
   "FIRE": false,
   "DROWNING": false,
   "FALL": false
}
```

### Damage Attributes

| Attribute     | Description                                              | Value      |
|---------------|----------------------------------------------------------|------------|
| `BLOCK_EXPLOSION`        | Damage caused by being in the area when a block explodes.       | Boolean    |
| `CONTACT`        | 	Damage caused when an entity contacts a block such as a Cactus.       | Boolean    |
| `CRAMMING` | Damage caused when an entity is colliding with too many entities.   | Boolean    |
| `DRAGON_BREATH`        | Damage caused by a dragon breathing fire.       | Boolean    |
| `DROWNING`        | 		Damage caused by running out of air while in water.       | Boolean    |
| `ENTITY_ATTACK` | Damage caused when an entity attacks another entity.   | Boolean    |
| `ENTITY_EXPLOSION`        | 	Damage caused by being in the area when an entity explodes.       | Boolean    |
| `ENTITY_SWEEP_ATTACK`        | 	Damage caused when an entity attacks another entity in a sweep attack.       | Boolean    |
| `FALL` | 	Damage caused when an entity falls a distance greater than 3 blocks.   | Boolean    |
| `FALLING_BLOCK`        | 	Damage caused by being hit by a falling block which deals damage.       | Boolean    |
| `FIRE`        | 			Damage caused by direct exposure to fire.       | Boolean    |
| `FIRE_TICK` | Damage caused due to burns caused by fire.   | Boolean    |
| `FLY_INTO_WALL`        | 	Damage caused when an entity runs into a wall.       | Boolean    |
| `HOT_FLOOR`        | 		Damage caused when an entity steps on Magma.       | Boolean    |
| `LAVA` |  Damage caused by direct exposure to lava.   | Boolean    |
| `LIGHTNING`        | 	Damage caused by being struck by lightning.       | Boolean    |
| `MAGIC`        | 				Damage caused by being hit by a damage potion or spell.       | Boolean    |
| `POISON` | 	Damage caused due to an ongoing poison effect   | Boolean    |
| `PROJECTILE`        | 			Damage caused when attacked by a projectile.       | Boolean    |
| `STARVATION` | Damage caused by starving due to having an empty hunger bar  | Boolean    |
| `SUFFOCATION`        | 	Damage caused by being put in a block.       | Boolean    |
| `SUICIDE`        | 		Damage caused by committing suicide using the command "/kill".       | Boolean    |
| `THORNS` | 	Damage caused in retaliation to another attack by the Thorns enchantment.   | Boolean    |
| `VOID`        | 			Damage caused by falling into the void       | Boolean    |
| `WITHER` | 	Damage caused by Wither potion effect   | Boolean    |

<span class="label label-note">Note</span> You may use spaces and lowercase letters (e.g `fly into wall`)

<span class="label label-note">Note</span> `DRYOUT`, `MELTING`, and firework damage does not work on players.
