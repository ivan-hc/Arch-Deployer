# Arch-Deployer
A script to bulk download an Arch Linux package with all its dependencies.

--------------------------------------------------------------------
- [Installation methods](#installation-methods)
     - [Using "AM"](#1-am-application-manager) (recommended)
     - [Using "wget" (locally)](#2-wget-the-script-directly)
     - [Using your favourite AUR helper](#3-arch-user-repository-aur)
- [Usage](#usage)
- [Related Projects](#related-projects)
--------------------------------------------------------------------
# Installation methods
To obtain the script you can run multiple methods, the main three are:
 1. [Using "AM", the Application Manager](#1-am-application-manager) (recommended)
 2. [Using "wget" (locally)](#2-wget-the-script-directly)
 3. [Using your favourite AUR helper](#3-arch-user-repository-aur)

### 1. "AM" APPLICATION MANAGER
I recommend using "[AM" Application Manager](https://github.com/ivan-hc/AM-application-manager)", because it can easilly keep you updated with the latest version of all the programs managed, and without root permissions ("sudo" is needed only to install/remove the programs):
   - TO INSTALL ARCH-DEPLOYER
    
         sudo am -i arch-deployer
   - TO UPDATE IT (without "sudo", this command will also update other programs managed by "AM")
    
         am -u
   - TO REMOVE IT:
   
         sudo am -r arch-deployer     
### 2. WGET THE SCRIPT DIRECTLY
You can obtain and run the script locally, this way:
   
       wget https://raw.githubusercontent.com/ivan-hc/Arch-Deployer/main/arch-deployer
       chmod a+x ./arch-deployer
Perform the same commands periodically to get the latest versio of this script.

### 3. ARCH USER REPOSITORY (AUR)
A [third-party script on AUR](https://aur.archlinux.org/packages/arch-deployer-git/) is also available, using our favorite AUR helper, ie
    
         paru -S arch-deployer-git

NOTE: I'm not the maintainer of any AUR package (method 3), more updated versions are only available using "AM" (method 1) or wget (method 2). You choose.

# Usage
If you have downloaded it locally (see the method 2, above):

    ./arch-deployer $PROGRAM

If you have installed Arch-Deployer from "AM" (method 1) or AUR (method 3):

    arch-deployer $PROGRAM
  
At the end of the process, all the packages will be extracted and the folders placed into an .AppDir directory, so you can work on an AppImage.

# Related projects
##### Sources and tools
- libunionpreload from https://github.com/project-portable/libunionpreload
- appimagetool from https://github.com/AppImage/AppImageKit

##### This project is heavily inspired by
- pkg2appimage, at https://github.com/AppImage/pkg2appimage

### Arch-Deployer is part of "AM"
the multi-architecture Application Manager for any GNU/Linux distribution, find out more at
# [github.com/ivan-hc/AM-application-manager](https://github.com/ivan-hc/AM-application-manager)
