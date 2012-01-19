For Live branch only, not all components need updating all the time, version number here refers to the library/DLL.

##0.7.0 (upcoming)
  * [WEB] Option to enable/disable public website
  * [WEB] View, delete and add to white/ban lists
  * [WEB] Restart when free scheduled job
  * [WEB] Delete servers
  * [WEB] Delete world and optionally set a random seed

##0.6.4 (current)
  * [DLL] Biome Extractor isn't exiting properly if 1.1 client is installed so stop it running automatically

##0.6.3
  * [WEB] fix inability to add bukkit in certain circumstances
  * [WEB] Scheduled jobs interface wasn't refreshing when deleting a job

##0.6.2
  * [DLL] Trim log messages over 255 characters

##0.6.1
  * [APP] Add backup external IP checker in case icanhazip.com is down

##0.6.0
  * [WEB] Dynamic DNS with yams.in address
  * [WEB] New connections tab shows what to send to your users so they can connect
  * [WEB] Display player position (slow update)
  * [WEB] Fix for repeating log entries when lots come in at once
  * [DLL] Change Bukkit and overviewer URLs
  * [APP] Reset ports button in updater
  * [DLL] Fix crash when user tries to log in twice

##0.5.0 
  * [WEB] Interface for creating and running multiple servers
  * [WEB] Right-click context menu for players (give, teleport, PM, ban etc)
  * [WEB] Buttons to toggle rain/snow and set time
  * [APP] Scheduled job to clear out old log data

##0.4.0
  * [WEB] Allow turning off/on port forwarding and firewall opening
  * [WEB] Allow setting of Listen IP and port for Web interfaces
  * [WEB] Allow setting IP and port for MC Server
  * [DLL] Better reporting of player numbers
  * [WEB] Log out button
  * [WEB] Redesigned and refactored around jQuery web interface
  * [WEB] Creation and deletion of scheduled tasks through the interface

##0.3.2
  * [DLL] Fix for world folder being in the wrong place.

##0.3.1
  * [DLL] Detects a corrupted jar download and forces and re-download

##0.3.0
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