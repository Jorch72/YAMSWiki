# Branches
## gh-pages
This is for the public website (http://richardbenson.github.com/YAMS/), and not directly related to the operation of YAMS.
## updater
This branch is read by the service when doing automatic updates, files in the root are "live" and the "dev" folder contains the files used in the development branch of updating.  See [[Update Mechanism]] for a guide on how this works.
## 0.x
Contains the workings for the next live version.  New features go in here and only in here.  Once a version is merged to master and made live, a new 0.x branch should be created for working on the next set of features.
## master
The currently live version of YAMS is always here, left clean for quick bug fixes.  The only changes made to this branch should be for fixing bugs found in the latest feature release.  Once a feature release is ready, it is merged into this branch and then becomes the live version.

# Master Structure
* __Binaries__ - Should be empty in git, will be filled by VS2010
* __Source__ - The Visual Studio 2010 Solution and sub-projects
    * __VS 2008 Interops__ - These are needed purely to generate the UPnP DLLs as there is a bug in VS2010 and .NET 3.5 meaning these Interops are not built correctly.
    * __YAMS-Library__ - Core DLL that contains any functions that actually do something
    * __YAMS-Service__ - The Windows service that keeps YAMS going 24/7
    * __YAMS-Setup__ - Visual Studio setup project for creating the MSI to distribute
    * __YAMS-Tester__ - A throw-away app for checking various functions before they go into the service
    * __YAMS-Updater__ - Small app to restart the service and apply updates to core files
    * __YAMS-Web__ - VS2010 Web Project for web files

# Building and testing
As YAMS is a service, building and debugging is a pain.  My preferred method of working is as follows:

  1. Install YAMS from the web and allow to update.
  2. Log in to admin console and set default server not to auto start (Settings tab)
  3. Stop the service from MMC (services.msc) and set to Manual start.
  4. Delete the web folder, open a command window as an administrator
  5. CD to the YAMS directory and create a symbolic link for the web directory: "mklink /D web C:\Full\path\to\YAMS-Web"

Once this is set up, on build you do the following:

  1. Stop the service
  2. Build the file and copy over the top of the one in Program Files
  3. Start the service

When working on the web files, all you need do is save and do a full refresh.  Most browsers seem to ignore full refreshes when a script downloads another script, and this second script is still served from cache.  To combat this, use the [Empty Cache Button](https://addons.mozilla.org/en-us/firefox/addon/empty-cache-button/) Firefox extension.