# Commands and Permissions

### broadcast
**Alias:** `tgm.broadcast`<br>
**Permission Node:** bc<br>
**Usage:** `broadcast [list|preset|raw|playerpreset|playerraw|config|start|stop|reload]`
<hr>

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
