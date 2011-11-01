# Branches
## gh-pages
This is for the public website (http://richardbenson.github.com/YAMS/), and not directly related to the operation of YAMS.
## updater
This branch is read by the service when doing automatic updates, files in the root are "live" and the "dev" folder contains the files used in the development branch of updating.  See [[Update Mechanism]] for a guide on how this works.
## 0.x
Contains the workings for the next live version.  New features go in here and only in here.  Once a version is merged to master and made live, a new 0.x branch should be created for working on the next set of features.
## master
The currently live version of YAMS is always here, left clean for quick bug fixes.  The only changes made to this branch should be for fixing bugs found in the latest feature release.  Once a feature release is ready, it is merged into this branch and then becomes the live version.