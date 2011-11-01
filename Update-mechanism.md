# Update mechanism
Almost everything the updater needs is contained in [AutoUpdate.cs](https://github.com/richardbenson/YAMS/blob/master/Source/YAMS-Library/Functions/AutoUpdate.cs) and the CheckUpdates() function does the regular updates.

## Version file
As part of the process, a json file is downloaded from the updater repository ([versions.json](https://github.com/richardbenson/YAMS/blob/updater/versions.json)) which gives some additional information for YAMS to decide if an update is needed.  Originally this was solely intended for the version numbers of external apps, as they usually included the version in the file name itself.  So to avoid pushing a full YAMS update whenever an external updated, the JSON file could be updated and YAMS would see that a new version was available.  This has been extended to include the download and updating of external DLLs required by YAMS.  The mechanism now in place allows for new DLLs to be downloaded in advance of the full YAMS update that requires them.

## Minecraft itself
YAMS uses either an eTag or Last-Modified HTTP header to determine if an update is required to the JAR (and most other files in fact) to reduce the need to download and then compare to check if the file has been updated (as was the case in the last MC project I worked on).  As these downloads can sometimes become corrupted, there is an additional option on CheckUpdates() that forces the re-download of all JAR files if the console outputs a specific error message.  This same procedure is used for downloading Bukkit if requested.

As part of the process of checking for Minecraft updates, another JSON file is downloaded ([properties.json](https://github.com/richardbenson/YAMS/blob/updater/properties.json)) that describes all the settings available within the Minecraft server itself.  Again this is designed in such a way that this is the only file that needs updating if Notch adds additional options to the server.properties file.

## YAMS updates
YAMS can download each of its components seperately, the checks are done in this order:
  1. YAMS-Library.dll
  2. YAMS-Service.exe
  3. Web
  4. YAMS-Updater.exe
  5. DLLs in /lib

The Library and service are written to a .UPDATE file, which the Updater will rename on a /restart command.  The web site is downloaded as a zip (to avoid checking all the files individually) which is then extracted over the top of the existing web site.

## External apps
External apps are checked in the same way, except the URLs for each are hard-coded in with a variable to replace for the version number.  These are usually a zip file that is extracted over the top of the old version.  Detection for 32/64-bit is included where the app provides binaries for both.

## Applying updates
The last stage is determining if there are updates, what needs to be restarted and is it safe to do so.  YAMS will not restart itself or a server if there are any players currently connected.