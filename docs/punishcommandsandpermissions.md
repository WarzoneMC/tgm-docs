# Punish Commands

### punish
Opens a punishment interface.<br>
**Alias:** pun, pg, pgui<br>
**Usage:** `punish [player|reload]`
>#### punish reload
Reloads all punishment presets.

<hr>

### chat
Controls the Server chat channel.<br>
**Permission Node:** `tgm.chat.control`<br>
**Usage:** `chat [mute|clear]`<br>
<span class="label label-note">Note</span> /chat conflicts with MultiChat, need a /c Alias.
<hr>

### report
Report a player.<br>
**Usage:** `report [player] [reason]`<br>
<hr>

### reports
View all recent reports.<br>
**Permission Node:** `tgm.reports`<br>
**Usage:** `reports [page]`
<hr>

### alts
Lookup the alternate accounts of a targeted username.<br>
**Permission Node:** `tgm.lookup`<br>
**Usage:** `alts [username]`
<hr>

### punishments
Lists all punishments that the targeted player has.<br>
**Alias:** p<br>
**Permission Node:** `tgm.punish.list`<br>
**Usage:** `punishments [player]`
<hr>

### lookup
Get information on the targeted player.<br>
**Alias:** lu<br>
**Permission Node:** `tgm.lookup`<br>
**Usage:** `lookup [player]`
<hr>

### lookupip
Get information on the ip address.<br>
**Alias:** luip<br>
**Permission Node:** `tgm.lookup`<br>
**Usage:** `lookupip [ip]`
<hr>

### ban-ip
Ban a player by IP address.<br>
**Alias:** banip<br>
**Permission Node:** `tgm.punish.ban-ip`<br>
**Usage:** `ban-ip [username/ip] [length] [reason]`
<hr>

### ban
Ban a player.<br>
**Permission Node:** `tgm.punish.ban`<br>
**Usage:** `ban [username] [length] [reason]`
<hr>

### kick
Kick a player.<br>
**Permission Node:** `tgm.punish.kick`<br>
**Usage:** `kick [username] [reason]`
<hr>

### mute
Mute a player.<br>
**Permission Node:** `tgm.punish.mute`<br>
**Usage:** `mute [username] [length] [reason]`
<hr>

### warn
Warn a player.<br>
**Permission Node:** `tgm.punish.warn`<br>
**Usage:** `warn [username] [reason]`
<hr>

### revert
Revert an existing punishment.<br>
**Permission Node:** `tgm.punish.revert`<br>
**Usage:** `revert [id]`
