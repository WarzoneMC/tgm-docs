# Match Commands

### maps
View the maps that are on Warzone, although not necessarily in the rotation.<br>
**Usage:** `maps [type] [page]`
<hr>

### findmaps
Find the maps that are on Warzone, although not necessarily in the rotation.<br>
**Usage:** `maps [map name] [page]`
<hr>

### rotation
View all of the maps in the current rotation.<br>
**Alias:** rot<br>
**Usage:** `rotation [page]`
<hr>

### rotations
View all of the rotations currently in the repository.<br>
**Alias:** rots<br>
**Usage:** `rotations`
<hr>

### setrotation
Sets the current rotation.<br>
**Permission Node:** `tgm.command.setrot`<br>
**Alias:** setrot<br>
**Usage:** `setrotation [rotation]`
<span class="label label-note">Note</span> Use /rotations to view the avaliable options.
<hr>

### cycle
Cycle to a new map.<br>
**Permission Node:** `tgm.cycle`<br>
**Usage:** `cycle`
<hr>

### start
Start the match.<br>
**Permission Node:** `tgm.start`<br>
**Usage:** `start`
<hr>

### end
End the match.<br>
**Alias:** finish<br>
**Permission Node:** `tgm.end`<br>
**Usage:** `end`
<hr>

### cancel
Cancel all active countdowns.<br>
**Permission Node:** `tgm.cancel`<br>
**Usage:** `cancel`
<hr>

### setnext
Set the next map.<br>
**Alias:** sn<br>
**Permission Node:** `tgm.setnext`<br>
**Usage:** `setnext [map name]`
<hr>

### classes
Opens a menu to view all classes available<br>
**Usage:** `classes`
<hr>

### class
Choose a class.<br>
**Usage:** `class [kit name]`
<hr>

### join
Join a team.<br>
**Alias:** play<br>
**Usage:** `join`
<hr>

### killstreak
See yours or another players current killstreak.<br>
**Alias:** ks<br>
**Usage:** `killstreak [player]`
<hr>

### teleport
Teleport to a player.<br>
**Permission Node:** `tgm.teleport`<br>
> Allows staff members to teleport outside of Spectator.

**Alias:** tp<br>
**Usage:** `teleport [player]`
<hr>

### team
Manage teams.<br>
**Permission Node:** `tgm.team`<br>
**Usage:** `team [alias|force|size]`

>#### alias [team] [name]
Select a team and give the team a new name.

>#### force [player] [team]
Force the selected player to join the selected team.

>#### size [team] [minimum] [maximum]
Select a team and set a minimum and maximum amount for team sizes.

<hr>

### loadmaps
Refreshes the map library and rotation from the repository.<br>
**Permission Node:** `tgm.loadmaps`<br>
**Usage:** `loadmaps`
<hr>

### channel
Change or select a chat channel.<br>
**Permission Node:** `tgm.teleport`<br>
**Alias:** chatchannel, cc<br>
**Usage:** `channel [all|team|staff]`
<hr>

### channel
Change or select a chat channel.<br>
**Usage:** `channel [all|team|staff]`
<hr>

### t
Send a message to your team.<br>
**Usage:** `t [message]`

### next
View the next map in the rotation.<br>
**Usage:** `next`
<hr>

### map
View the map info for the current map.<br>
**Usage:** `map`
<hr>

### time
See the time elapsed currently for the match.<br>
>#### time [limit] [seconds]
Limit the amount of time the current match has remaining.

<hr>

### config
Edit the configuration.<br>
**Permission Node:** `tgm.config`<br>
**Usage:** `config [stats|reload]`
>#### config stats [on|off]
Toggle stat tracking.

>#### config reload
Reload all configuration.

<hr>

### leaderboard
List the top 10 players on the Server.<br>
**Alias:** lbm lboard<br>
**Usage:** `leaderboard [type]`

>#### leaderboard type [kills|wins|losses|xp]

<hr>

### stats
Display your stats.<br>
**Alias:** stat<br>
**Usage:** `stats [player]`

<hr>

### countdown
Manage custom countdowns.<br>
**Permission Node:** `tgm.countdown`<br>
**Alias:** cd<br>
**Usage:** `countdown [list|start|create|edit|cancel]`
>#### countdown list
Lists all registered countdowns.

>#### countdown start [id]
Start the countdown with the id specified.

>#### countdown create [id] [time] [title] [color] [style] [visable] [invert] [teams] [onFinish]
<span class="label label-note">Note</span> Unsure what countdown create should be documented.
