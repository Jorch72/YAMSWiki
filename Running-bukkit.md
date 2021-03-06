##Setting your server to run Bukkit
* Click Settings > Installed Apps
* Check "Bukkit" and save
* Click Settings > Run Updates now
* Stop your server (right-hand panel)
* Settings tab, change server type to Bukkit, save
* Start your new Bukkit server

##Installing plugins
(Based on the [Official Bukkit plugin install guide](http://wiki.bukkit.org/Installing_Plugins))

* Download a plugin of your choice.
* If your server is currently running, click stop in the "Control" section of the right panel
* Place the .jar and any other files in the plugins directory for that specific server (i.e. you first server will be in <install dir>/servers/1/).
* Start the server and wait for it to be fully loaded
* Press Stop again to bring the server to a clean stop.
* Start your server again.
* All done! Your plugin should be installed and ready to be used.

##Backups
As of 0.8, YAMS will backup any folder that starts with "world" to cater for the default Bukkit world locations; "world", "world_nether" and "world_the_end".  If you are using a multi-world plugin and want your extra worlds to be included in the backup, make sure they start with "world" (e.g. "world_skylands", "world_aether" etc.)