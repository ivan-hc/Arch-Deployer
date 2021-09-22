# Arch-Deployer
A script to bulk download an Arch Linux package with all its dependencies.

# Usage
1. Download the script:  `wget https://raw.githubusercontent.com/ivan-hc/Arch-Deployer/main/arch-deployer`
2. Copy the name of the program you wish and all its dependences from [archlinux.org/packages](https://archlinux.org/packages/)
3. Paste all the words on `SAMPLE` at the line 10 of the script, this way: `"program" "dep1" "dep2" "dep3"...`
4. Replace `SAMPLE` at line 3 with the name of the program
5. Made the script executable:  `chmod a+x ./arch-deployer`
6. Run the script:  `./arch-deployer`

At the end of the process, all the packages will be extracted and the folders placed into an .AppDir directory, so you can work on an AppImage.
