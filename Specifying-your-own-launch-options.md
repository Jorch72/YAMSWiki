(available in 0.8 onwards)
##Basic use
You can override the default launch parameters by placing a file named `args.txt` in the server's folder.  This will override **ALL** of the arguments, including the path to the JAR and other settings designed to make Minecraft run as optimally as possible.  When working with this file, it is best to start with the arguments that are already in use and you can retrieve these from the main server console.  Whenever a server is started, a line is output showing the arguments used, such as:

    -server -XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:+CMSIncrementalPacing -XX:ParallelGCThreads=1 -XX:+AggressiveOpts -Xmx1024M -Xms1024M -jar "C:\Program Files (x86)\YAMS\lib\minecraft_server.jar" nogui

Copy and paste this into your new `args.txt` file and edit accordingly.  If you break your server, simply delete or rename the `args.txt` file and YAMS will go back to default settings.  Using this file will render the jar, memory and optimisation settings useless.

##Running other server jars
This does open the opportunity to run additional jars than the three that YAMS supports, simply replace the `-jar` argument with the location of your custom jar.  It makes sense to keep it in the same folder as the other jars but give it a different name than "minecraft_server.jar" (or the others in there) as otherwise it will be overwritten every update.