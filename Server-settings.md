![YAMS server settings](http://yams.in/assets/images/docs/server-log-settings.png)

The server settings screen contains all the options for configuring your server and the world inside it.  It is split up into two parts; Server Settings and Server Properties.

## Server Settings

  * **Title**: This is used only inside YAMS in the [[servers menu]] and in the header.
  * **Java Optimisations**: If you have the [JDK](http://www.oracle.com/technetwork/java/javase/downloads/jdk-7u2-download-1377129.html) installed then YAMS will use that over the JRE and apply a few extra command line parameters to make the server run a little smoother.
  * **Assigned Memory**: How much memory to assign to this server.  This is a Java setting and seems to mostly affect virtual memory and not RAM usage.
  * **Auto Start Server**: Whether to start this server up automatically whenever YAMS is started.
  * **Type**: One of three options:
    * **Vanilla**: The official released version of Minecraft server.
    * **Bukkit**: CraftBukkit based server. (make sure you have ticked bukkit in the [[installed apps]] menu)
    * **Vanilla pre-release**: Official weekly snapshots which may be buggy and will require a pre-release client as well, use only if you know what you are doing.
  * **MOTD**: Message of the day broadcast when a user logs on.
  * **Port**: The port number to run the server on (default 25565).  This can usually be left alone, when you add a new server YAMS will look for the next available port so there shouldn't be any conflicts.
  * **Listen IP**: The IP that the server listens on, usually this won't need changing, but if you have multiple IP addresses on your system you may need to select the correct one here.  This is **NOT** the IP address you should give to anyone you want to connect to your server from outside your network, see the [[server connections]] tab for more details.

## Server Properties

These are the settings as contained in Minecraft's [server.properties](http://www.minecraftwiki.net/wiki/Server.properties), explanations of each setting can also be gained by hovering over the title.  As additional settings are added, this will update itself without needing a new YAMS version.
