Listed here are features that aren't yet in YAMS but are either planned or have been asked for, if there is something you want that isn't listed, please put it on as an [issue](https://github.com/richardbenson/YAMS/issues).  Remember, YAMS will never mod the Minecraft server, it is an admin tool.

## Partial
The following are partially implemented and may just need some UI work to finish off

  * MOTD (works but can't yet be changed)
  * User levels
  * Task scheduler for all jobs
  * Overviewer rendering (can be triggered manually with a POST request)
  * C10t rendering (Can be triggered with a JavaScript console)

## Planned
These are features YAMS will **definitely** have:

  * Upload and download of world
  * Automatic backup to Zip/Tar/etc with retention policies and access from the admin panel to your backups
  * Upload and support of plugins (either bukkit or official mod support)

## Possible
These are features that YAMS _may_ have one day:

  * Bukkit support: Once it's stable and officially released, as long as Mojang don't get mod support out before then
  * Open your computer's firewall ports when needed and closed again when not
  * Automated UPnP port mapping
  * Optional embedded Mumble server (Murmur) per Minecraft server

## Never
The following things will never be implemented in YAMS:

  * Intentional backdoors, or elevated privileges for developers
  * Wrapper mode: Your Minecraft client will always be talking directly to the Minecraft server (Mojang or Bukkit)