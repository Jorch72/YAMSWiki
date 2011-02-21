The setup launcher should check for and install any additional dependencies you need for YAMS to run on your system, one of which is SQL Compact Edition.  This is not to be confused with SQL Express and does not run as a service, it is merely a driver for accessing the included flat file database.

By default YAMS installs itself to your "Program Files" folder.  On a 64-bit system this is "Program Files (x86)" even though as a .NET application it will run in whatever "bitness" your system is and any add-ons will be downloaded as the right version for your system.  This is also where your server worlds will be kept, along with any output from add-ons.

Once installed it registers a service on your computer called "YAMS".

There are no registry entries required, all setting information is kept in the internal DB.