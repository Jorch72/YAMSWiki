One way would be to create a [symbolic link](http://en.wikipedia.org/wiki/NTFS_symbolic_link) in the directory to your new world.  This means YAMS should see it as a normal directory and then back it up, would just need renaming if you ever restored it. (assumes you are on Windows Vista/2008+)

Do the following on the server (replace `skyisland` with the folder name you want to backup):

  * Open a cmd prompt as administrator
  * CD to the server directory (C:\program files (x86)\YAMS\servers\1\ by default)
  * Type `mklink /D world_skyisland skyisland`
  * Run a backup through admin
  * Open the zip and check you have the new folder and that it contains the right files