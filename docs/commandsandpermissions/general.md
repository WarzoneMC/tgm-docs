# General Commands

### broadcast
**Alias:** bc<br>
**Permission Node:** `tgm.broadcast`<br>
**Usage:** `broadcast [list|preset|raw|playerpreset|playerraw|config|start|stop|reload]`
>#### list
Lists all of the preset broadcast messages.

>#### preset [id] [args]
List the message contents of the present set in [id].

>#### raw
Send your own message using chat colours.

>#### playerpreset
Alias: ppreset
Send a preset broadcast message to the targeted player.

>#### playerraw
Send your own message using chat colours to the targeted.

>#### config [autobroadcast|interval|url|queue]
autobroadcast: toggle auto broadcast (boolean)<br>
interval: change the amount of time (in seconds) when a message broadcasts (integer)<br>
url:<br>
queue:<br>
<span class="label label-note">Note</span> Unsure what url and queue do.

>#### start
Starts the auto broadcast task.

>#### stop
Stops the auto broadcast task.

>#### reload
Reloads the auto broadcast task.

<hr>

### ping
Checks a players ping.
**Usage:** `ping [player]`
<hr>

### tgm
Displays essential server information.
**Permission Node:** `tgm.command.tgm`<br>
**Usage:** `ping [player]`
<hr>

### profilecache
Clear the profile cache.
**Permission Node:** `tgm.command.profilecache`<br>
**Usage:** `profilecache clear`
<hr>

### nicks
View all nicknamed players.
**Permission Node:** `tgm.command.whois`<br>
**Usage:** `profilecache clear`
<hr>

### whois
Views nickname and identity of a targeted player.
**Permission Node:** `tgm.command.whois`<br>
**Usage:** `whois [player]`
<hr>

### nick
View all nicknamed players.
**Permission Node:** `tgm.command.nick`<br>
**Usage:** `nick [set|reset|skin|stats|rank] [rank]`

<span class="label label-note">Note</span><br>
You cannot set your name as someone else who is currently online.<br>
Your nickname must be shorter than 16 characters.<br>
Need to reconnect for the changes to fully apply.

>#### set [name]
**Alias:** name<br>
Set your nickname.

>#### reset
Revert your nickname back to original username.

>#### skin [name]
Set your skin to the specified username.

>#### stats [statName|good|random|bad|new] [option]
Set stats for user.<br>
**statName**: Change an particular statistic.<br>
**good**: Set statistics to a Good bar.<br>
**bad**: Set statistics to a bad bar.<br>
**random**: Set statistics randomly.<br>
**new**: Set statistics to a clean slate.<br>

>#### rank [rank]
Set a rank on nicked player.

### tag
View all nicknamed players.
**Alias:** tags<br>
**Usage:** `tag`

>#### set [tag] [player]
**Permission Node:** `tgm.tags.set`<br>

>#### add [tag] [player|UUID]
**Permission Node:** `tgm.tags.add`<br>

>#### remove [tag] [player|UUID]
**Permission Node:** `tgm.tags.remove`<br>

>#### list [tag] [player|UUID]
**Permission Node:** `tgm.tags.list`<br>
