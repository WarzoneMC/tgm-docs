# Gamerules

This module is used to modify gamerules native to Minecraft.

## Example

```json
	"gamerules": {
		"keepInventory": true,
		"doDaylightCycle": true,
		"doWeatherCycle": false
	},
```

### Gamerules Attributes

| Attribute | Description                                                           | Value    | Default |
|-----------|-----------------------------------------------------------------------|----------|---------|
| `announceAdvancements`   | Whether advancements should be announced in chat. | Boolean     | False     |
| `commandBlockOutput`   | Whether command blocks should notify admins when they perform commands. | Boolean     | False     |
| `disableElytraMovementCheck`  | Whether the server should skip checking player speed when the player is wearing elytra.  | Boolean     | True           |
| `disableRaids`   | Whether raids are disabled. | Boolean     |      |
| `doDaylightCycle`  | Whether the day-night cycle and moon phases progress.  | Boolean     | False          |
| `doEntityDrops`   | Whether entities that are not mobs should have drops. | Boolean     |      |
| `doFireTick`  | Whether fire should spread and naturally extinguish.  | Boolean     |           |
| `doInsomnia`   | Whether phantoms can spawn in the nighttime. | Boolean     |     |
| `doImmediateRespawn`  | Players respawn immediately without showing the death screen.  | Boolean     |           |
| `doLimitedCrafting`  | Whether players should be able to craft only those recipes that they've unlocked first.  | Boolean     |           |
| `doMobLoot`  | Whether mobs should drop items.  | Boolean     |           |
| `doMobSpawning`   | Whether mobs should naturally spawn. Does not affect monster spawners. | Boolean     | False    |
| `doTileDrops`  | Whether blocks should have drops.  | Boolean     |           |
| `doWeatherCycle`  | Whether the weather can change.  | Boolean     | False          |
| `drowningDamage`  | Whether the player should take damage when drowning.  | Boolean     |           |
| `fallDamage`  | Whether the player should take fall damage.  | Boolean     |           |
| `fireDamage`  | Whether the player should take fire damage.	  | Boolean     |           |
| `keepInventory`  | Whether the player should keep items in their inventory after death.  | Boolean     | False          |
| `logAdminCommands`  | Whether to log admin commands to server log.	  | Boolean     | False          |
| `maxCommandChainLength`  | Determines the number at which the chain command block acts as a "chain".  | Value     |          |
| `maxEntityCramming`  | The maximum number of other pushable entities a mob or player can push, before suffocating.	  | Value     |           |
| `mobGriefing`  | Whether or not mobs can interact with the environment.  | Boolean     |           |
| `naturalRegeneration`  | Whether the player can regenerate health naturally.	  | Boolean     |           |
| `randomTickSpeed`  | How often a random block tick occurs.  | Value    |           |
| `reducedDebugInfo`  | Whether the debug screen shows all or reduced information.	  | Boolean     |           |
| `sendCommandFeedback`  | Whether the feedback from commands executed by a player should show up in chat.  | Boolean     |           |
| `showDeathMessages`  | Whether death messages are put into chat when a player dies.	  | Boolean     |           |
| `spawnRadius`  | The radius players spawn at the default world spawn point.	  | Value    |           |
| `spectatorsGenerateChunks`  | Whether players in spectator mode can generate chunks.	  | Boolean     |           |

<span class="label label-note">Note</span> `doImmediateRespawn` should not be used to modify respawning; use `respawn` module.

<span class="label label-note">Note</span> `doTileDrops` should not be used to modify drops; use `itemremove` module.

<span class="label label-note">Note</span> `drowningDamage`, `fallDamage`, `fireDamage` should not be used to disable damage; use `damageControl` module.
