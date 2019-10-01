# Damage Control

This module is used to determine whether or not damage is taken as a result of various player actions.

## Example

```json
"damageControl": {
   "fire": false,
   "suffocation": false,
   "fall": false
}
```

### Damage Attributes

| Attribute     | Description                                              | Value      |
|---------------|----------------------------------------------------------|------------|
| `fire`        | Whether or not a player takes damage when on fire.       | Boolean    |
| `fall`        | Whether or not a player takes damage when falling.       | Boolean    |
| `suffocation` | Whether or not a player takes damage upon suffocation.   | Boolean    |
