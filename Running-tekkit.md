To run a Tekkit server:

1. Log into YAMS admin console.
2. Head to "Settings" tab.
3. In the "Type" field, select "CraftBukkit".
4. Go back to the "Console" tab.
5. Click the "start" button and watch the main console window.
6. Look for a line that starts "Server Started: ", it will be something like this `Server Started: -server -XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:+CMSIncrementalPacing -XX:ParallelGCThreads=1 -XX:+AggressiveOpts -Djline.terminal=jline.UnsupportedTerminal -Xmx1024M -Xms1024M -jar "C:\Program Files\YAMS\lib\craftbukkit.jar" nogui`
7. Copy everything after the first colon (:)
8. In the server's directory (e.g. C:\Program Files (x86)\YAMS\servers\1) create a new blank text file called "args.txt".
9. Paste everything you copied earlier into this file, something like: `-server -XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:+CMSIncrementalPacing -XX:ParallelGCThreads=1 -XX:+AggressiveOpts -Djline.terminal=jline.UnsupportedTerminal -Xmx1024M -Xms1024M -jar "C:\Program Files\YAMS\lib\craftbukkit.jar" nogui`
10. Download Tekkit Server (NOT Technic Launcher, that's for your PC).
11. Extract the Tekkit zip into the server folder where you created the args.txt file.
12. In the args.txt file, replace the Bukkit path (e.g. `C:\Program Files\YAMS\lib\craftbukkit.jar`) with just "Tekkit.jar".
13. Start your server through the admin.

You will have to manually update Tekkit whenever a new version is released.

**NB**: It seems there is a corrupt file in the 3.1.2 download for Tekkit, so replace or delete the "mods\mod_NetherOres.jar" file as this will stop Tekkit from running presently