# Welcome to the VN-MC-Server-Service wiki!

The VN-MC Server Service is a service that is intended to run a Minecraft server on a windows based computer with .NET Framework 4.0+ 

## Features:
* Run a Minecraft-based server as a windows service. This means you can run this headless on a windows computer as a background process. 

* Adds extended options to the JVM instance for better performance and stability while being fully user-customize-able.

* Runs your existing jar file and system Java install. 

* Fully supports auto restart plugins natively! Just install your restart plugin and leave the rest.  

### Watchdog v2 Engine Features:
* Makes sure your java process is running at a specified interval
* If the process is not found, then it will attempt to restart the server process
* After the specified failure count, it will stop the service

### Backup v1 Engine Features
* Backs-up all files in the Minecraft directory to the backups directory at specified intervals
* Keeps a log of all backup functions and errors


## FILES
* Install.txt
   Once extracted the INSTALL.txt file explains all steps and processes involved in installing this service 

* Changelog.txt
   Contains all relevant change information in all versions of this service. Fixes and updates 


# Follow the readme/changelog/install files carefully along with the installer. 

## Moving to v1.0.3 
   If you are moving to the 1.0.3 version, you must create a backup of your server files ONLY and remove the all the config and service files/folders before install. The will need to use the new config file in the latest version for all features to work properly.

   
