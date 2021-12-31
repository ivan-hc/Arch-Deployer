# Arch-Deployer
A script to bulk download an Arch Linux package with all its dependencies.

# Usage
1. Download the script:
  
     `wget https://raw.githubusercontent.com/ivan-hc/Arch-Deployer/main/arch-deployer`
     
2. Made the script executable:  

     `chmod a+x ./arch-deployer`

3. Run the script by adding the name of the program (for example `$PROGRAM`), this way:

     `./arch-deployer $PROGRAM`

At the end of the process, all the packages will be extracted and the folders placed into an .AppDir directory, so you can work on an AppImage.

# Related projects
##### Sources and tools
- libunionpreload from https://github.com/project-portable/libunionpreload
- appimagetool from https://github.com/AppImage/AppImageKit

##### This project is also inspired by
- pkg2appimage, at https://github.com/AppImage/pkg2appimage

# See also
"AM" the multi-architecture Application Manager for any GNU/Linux distribution https://github.com/ivan-hc/AM-application-manager
