To expand on the documentation slightly:

1. Set your server to "Craftbukkit" in the Settings tab
2. In the console look for the line that starts "Server Started: "
3. Copy all the text in this line after the ":"
4. Create a new file in the server directory (e.g. C:\Program Files (x86)\YAMS\servers\1) called "args.txt"
5. Paste the line you copied earlier into this file
6. Download Tekkit and extract the zip into the same server you put the args.txt file
7. in args.txt replace after "-jar" with just "Tekkit.jar"
8. Start your server through admin

**NB**: It seems there is a corrupt file in the 3.1.2 download for Tekkit, so replace or delete the "mods\mod_NetherOres.jar" file as this will stop Tekkit from running presently