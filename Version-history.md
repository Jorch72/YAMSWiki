For Live branch only, not all components need updating all the time, version number here refers to the library/DLL.

##0.3.0 (current)
  * [ALL] Add better handling of exceptions and logging to file (development branch emails errors)
  * [DLL] Opens ports on Windows firewall and closes them when done
  * [DLL] Attempts to port forward using UPnP (depends on router)
  * [WEB] Moving the scroll on any log away from the bottom stops auto-scroll, returning scroll to the bottom resumes auto-scrolling.
  * [DLL] Better handling if YAMS crashes but MC doesn't, will kill old processes left orphaned by a crash
  * [DLL] Updates for overviewer
  * [WEB] Chat tab was not showing messages from console
  * [WEB] Updates for playernames that have underscores and other characters
  * [APP] Shows if port forwards are working
  * [APP] Allows changing of admin and public ports
  * [DLL] Support for pre-release versions downloading, updating and switching between beta and pre
  * [WEB] Change settings in the server.properties

##0.2.3
  * [DLL] Clears player list on crash
  * [APP] Better handling if Java not installed on setup
  * [WEB] Server page now has some styling, can navigate from home page to individual server pages
  * [WEB] Bukkit checkbox wasn't saving state
  * [DLL] Move configuration files out of ./config folder as a lot of bukkit plugins can't handle this
  * [DLL] Show op users in player list
  * [DLL] Catch and store the game mode (creative/survival)
  * [DLL] Updates to the way files are downloaded from the net and better crash handling in this area
  * [DLL] Allow updating and addition of extra dlls as program expands and for security updates

##0.2.2
  * [DLL] Support for latest Overviewer (0.1.4) and 32/64-bit detection
  * [WEB] Will not request an update for the consoles if there is already one in place
  * [APP] Update all third party apps to latest
  * [DLL] Outputs from apps go to server's log, not global
  * [ALL] Sane version numbers
  * [DLL] Detect a server crash (i.e. non-safe process exit) and restart
  * [DLL] Copes better if admin port is in use (likely during a service restart)
  * [DLL] Potential support for tectonicus but needs a 3D device on the server
  * [WEB] Add default "admin" username to login screen
  * [DLL] Catch odd date returns in last modified field (coming from Bukkit.org)
  * [WEB] Show VM and RAM usage
  * [WEB] Change MOTD

##0.1.176
  * First publicly available version.