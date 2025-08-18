https://www.minecraft.net/en-us/download/server

Download minecraft_server..jar, rename it, and run it with the following command:

java -Xmx1024M -Xms1024M -jar minecraft_server.1.21.8.jar nogui

Should you want to start the server with its graphical user interface you can leave out the "nogui" part. Replacing "nogui" with "--help" might also be useful.

Might need a newer java version, such as "sudo apt install openjdk-21-jdk".

Edit server.properties
see https://minecraft.wiki/w/Server.properties

properties of interest:
difficulty
enforce-whitelist
force-gamemode - useful to forcibly switch gamemodes after changing the server settings after players have already joined... or maybe this happens automatically on reconnect, in which case what is the point?
gamemode - survival, creative, adventure, spectator
level-name
level-seed
motd
server-port
white-list

edit eula.txt

start server and run desired commands; commands of interest:
help
defaultgamemode
difficulty
gamemode
gamerule (see https://minecraft.wiki/w/Game_rule)
- keepInventory
- lavaSourceConversion
- maxEntityCramming
- maxExplosionDropDecay
- playersSleepingPercentage 30 is nice
seed
version
team might be interesting to allow/disallow friendly fire; compare with gamerule pvp
time
weather
transfer - this could be fun to make people hop between worlds
whitelist list
whitelist add playername
stop
