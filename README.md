
The VN-MC Server Service is a service that is intended to run a Minecraft server on a windows based computer with .NET Framework 4.0+ 

## Features:
* Run a Minecraft-based server as a windows service. This means you can run this headless on a windows computer as a background process. 

* Adds extended options to the JVM instance for better performance and stability while being fully user-customize-able.

* Runs your existing jar file and system Java install. 

* Default optimized for most Minecraft servers but has many options for user cutomizable options 

* Verifies Java version and server paths before each startup 

* Fully supports auto restart plugins natively! Just install your restart plugin and leave the rest. 

* Watchdog prevents a restart loop if there are configuration or system errors

* Detailed log file containing all serive relevant information

* Full backup of all server files automatically based on the given interval

### Watchdog v3 Engine Features:
* Protects your computer from unwanted failure loops either java or config related
    If the java process (server process) terminates, it will automatically restart. Watchdog v3 limits the number of times 
    the process can fail within the desired interval before shutting the service down


### Backup v2 Engine Features
* Backs-up all files in the Minecraft directory to the backups directory at specified intervals
* Keeps a log of all backup functions and errors (see changelog)
* If an OS shutdown is detected, an automatic backup is taken before the process is terminated incase something happens on restart (even if normal backups are disabled) 


## FILES
* Install.txt
   Once extracted the INSTALL.txt file explains all steps and processes involved in installing/uninstalling this service 

* Changelog.txt
   Contains all relevant change information in all versions of this service. Fixes and updates 


# Follow the readme/changelog/install files carefully along with the installer. 

## Moving to v1.1.0 
   If you are moving to the 1.1.0 version, you must create a backup of your server files ONLY and remove the all the config and service files/folders before install. The will need to use the new config file in the latest version for all features to work properly.
   SPECIFIC TO v1.1.0 Older config files are backward compatible, but are not advised as default options will be used and a warning        message will appear in the log file. 

## Known Issues
   Shutdown backup often doesnt complete properly because windows terminates the service without waiting. Has not corrupted any files in this process, but can often leave out the world folders, so its best to make sure you have the interval backup on just incase.  
