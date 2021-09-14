# Cvar list

<br>

> #### The following conventions are used to describe argument types:
> `string` - normal text characters  
> `integer` - whole numbers variable, e.g. 1, 2, 3, 4  
> `float` - floating point value variable, e.g. 1.0, 0.9, 0.8, 0.7  
> `bitflag` - binary digit whole value variable, e.g. 1, 2, 4, 8, 16, etc (or add 1+2 = 3, 1+2+4 = 7, etc)  

> #### Cvar color table  
`white` `red` `green` `blue` `yellow` `magenta` `cyan` `orange` `mdred` `mdgreen` `dkgreen` `mdcyan` `mdyellow` `mdorange` `mdblue` `ltgrey` `mdgrey` `dkgrey` `black`  

# Client  
#### Engine/renderer (cl/r)
| Cvar | Argument type | Value range | Default | Description |
|---------|---------------|-------------|---------|-------------|
| in_mouse | `integer` | `0-2`| `1` | Switch mouse input type between default and raw `(2)` |
| con_height | `float` | `0.1-1.0` | `0.5` | Change console height |
| cl_activateLean | `integer` | `0-1` | `1` | Toggle leaning when holding move keys and +activate |
| r_bloom | `integer` | `0-1` | `0` | Enable/disable bloom effect |

#### Mod (cg)
| Cvar | Argument type | Value range | Default | Description |
|---------|---------------|-------------|---------|-------------|
| cg_crosshairPulse | `integer` | `0-1` | `1` | Enable/disable pulsing of the crosshair. |
| cg_showFlags | `integer` | `0-1` | `1` | Enable/disable scoreboard coutnry flags |
| cg_bloodDamageBlend | `float` | `0.0-1.0` | `1.0` | Control blood blends when getting shot |
| cg_bloodFlash | `float` | `0.0-1.0` | `1.0` | Control blood flash when getting shot |
| cg_crosshairAlpha | `float` | `0.0-1.0` | `1.0` | Control crosshair opacity |
| cg_crosshairAlphaAlt | `float` | `0.0-1.0` | `1.0` | Control crosshair alt opacity |
| cg_crosshairColor | `string` | Color table | `white` | Change crosshair color |
| cg_crosshairColorAlt | `string` | Color table | `white` | Change crosshair color alt |
| ch_font | `integer` | `0-2` | `0` | Enable/disable OSP fonts |
| cg_drawWeaponIconFlash | `integer` | `0-1` | `0` |  Enable/disable weapon icon flashing when empty |
| cg_printObjectiveInfo | `integer` | `0-1` | `1` | Enable/disable printing of OBJ notifications in kill feed |
| cg_noChat | `integer` | `0-1` | `0` | Draw chat messages |
| cg_noVoice | `integer` | `0-1` | `0` | Draw and play voice chat messages |
| cg_drawPickupItems | `integer` | `0-1` | `1` | Draw item names upon pickup |
| cg_autoAction | `bitflag` | `0-1-2-4` | `0` | Control auto actions. `1` - record demo, `2` - take screenshot, `4` - dump stats file, `7` - all |
| cg_chatAlpha | `float` | `0.0-1.0` | `0.33` | Change chat background opacity |
| cg_chatBackgroundColor | `string` | `color table` | `""` | Change chat background color |
| cg_chatBeep | `integer` | `0-1` | `0` | Enable/disable chat sound notifications |
| cf_wstats | `float` | `0.0-99.0` | `1.2` | Change +wstats window scale |
| cf_wtopshots | `float` | `0.0-99.0` | `1.0` | Change +wtopshots window scale |
| cg_noAmmoAutoSwitch | `integer` | `0-1` | `0` | Enable/disable auto weapon switch when primary is out of ammo |
| cg_drawSpeed | `integer` | `0-4` | `0` | Draw speed meter. `1` - current only, `2` - current and top, `3` - current with accel color, `4` - current and top with accel color |
| cg_speedX | `integer` | `-999-999` | `315` | Change speed meter position in the horizontal axis |
| cg_speedY | `integer` | `-999-999` | `340` | Change speed meter position in the vertical axis |
| cg_tracers | `integer` | `0-3` | `1` | Draw bullet tracers. `1` - all, `2` - own only, `3` - other's only |
| cg_drawTriggers | `integer` | `0-1` | `1` | Draw objeective triggers (for Shoutcasters only) |
| cg_hitsounds | `bitflag` | `0-1-2-4` | `0` | Control hitsounds. `1` - headshot only, `2` - body only, `4` - team only, `7` - all |
| cg_hitsoundBodyStyle | `integer` | `1-9` | `1` | Change body hit sound |
| cg_hitsoundHeadStyle | `integer` | `1-11` | `1` | Change head hit sound |
| cg_spawnTimer_period | `integer` | `0-60` | `0` | [See here (use /timerset seconds)](https://www.youtube.com/watch?v=_NNYI8VbFyY) |
| cg_spawnTimer_set | `integer` | `-1-60` | `-1` | [See here (use /timerset seconds)](https://www.youtube.com/watch?v=_NNYI8VbFyY) |
| cg_drawReinforcementTime | `integer` | `0-3` | `1` | Draw respawn time. `1` - default, `2` - new, `3` - default and new |
| cg_reinforcementTimeColor | `string` | `color table` | `red` | Change respawn time color |
| cg_reinforcementTimeX | `integer ` | `-999-999` | `86` | Change default respawn time position in the horizontal axis |
| cg_reinforcementTimeY | `integer ` | `-999-999` | `70` | Change default respawn time position in the vertical axis |
| cg_reinforcementTimeProX | `integer ` | `-999-999` | `145` | Change new respawn time position in the horizontal axis |
| cg_reinforcementTimeProY | `integer ` | `-999-999` | `445` | Change new respawn time position in the vertical axis |
| cg_drawEnemyTimer | `integer` | `0-1` | `1` | Draw enemy timer. `1` - default, `2` - new, `3` - default and new |
| cg_enemyTimerColor | `string` | `color table` | `green` | Change enemy timer color |
| cg_enemyTimerX | `integer` | `-999-999` | `98` | Change default enemy timer position in the horizontal axis |
| cg_enemyTimerY | `integer` | `-999-999` | `60` | Change default enemy timer position in the vertical axis |
| cg_enemyTimerProX | `integer` | `-999-999` | `185` | Change new enemy timer position in the horizontal axis |
| cg_enemyTimerProY | `integer` | `-999-999` | `445` | Change new enemy timer position in the vertical axis |
| cg_findMedic | `integer` | `0-1` | `1` | Enable/disable camera lock at team medics when waiting for a revive |
| cg_zoomedSens | `float` | `0.0-99.0` | `.3` | Change sensitivity when scoped |
| cg_zoomedSensLock | `integer` | `0-1` | `0` | Enable/disable decreasing of sensitivity with each zoom step while scoped |
| cg_notifyTextX | `integer` | `-999-999` | `0` | Change kill feed position in the horizontal axis |
| cg_notifyTextY | `integer` | `-999-999` | `42` | Change kill feed position in the vertical axis |
| cg_notifyTextWidth | `integer` | `0-99` | `8` | Change kill feed char width |
| cg_notifyTextHeight | `integer` | `0-99` | `8` | Change kill feed char height |
| cg_chatX | `integer` | `-999-999` | `0` | Change chat position in the horizontal axis |
| cg_chatY | `integer` | `-999-999` | `385` | Change chat position in the vertical axis |
| cg_teamOverlayX | `integer` | `-999-999` | `640` | Change team overlay position in the horizontal axis |
| cg_teamOverlayY | `integer` | `-999-999` | `0` | Change team overlay position in the vertical axis |
| cg_compassX | `integer` | `-999-999` | `290` | Change compass position in the horizontal axis |
| cg_compassY | `integer` | `-999-999` | `420` | Change compass position in the vertical axis |
| cg_lagometerX | `integer` | `-999-999` | `585` | Change lagometer position in the horizontal axis |
| cg_lagometerY | `integer` | `-999-999` | `340` | Change lagometer position in the vertical axis |
| cg_drawFrags | `integer` | `0-1` | `1` | Enable/disable "you killed" frag center prints |
| cg_fragsY | `integer` | `-999-999` | `0` | Change frag center prints position in the vertical axis |
| cg_fragsWidth | `integer` | `-999-999` | `16` | Change frag center prints char width |