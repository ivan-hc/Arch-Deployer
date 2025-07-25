        ╭━━━┳━━━┳━━━┳╮╱╭╮╭━━━┳━━━┳━━━┳╮╱╱╭━━━┳╮╱╱╭┳━━━┳━━━╮
        ┃╭━╮┃╭━╮┃╭━╮┃┃╱┃┃╰╮╭╮┃╭━━┫╭━╮┃┃╱╱┃╭━╮┃╰╮╭╯┃╭━━┫╭━╮┃
        ┃┃╱┃┃╰━╯┃┃╱╰┫╰━╯┃╱┃┃┃┃╰━━┫╰━╯┃┃╱╱┃┃╱┃┣╮╰╯╭┫╰━━┫╰━╯┃
        ┃╰━╯┃╭╮╭┫┃╱╭┫╭━╮┃╱┃┃┃┃╭━━┫╭━━┫┃╱╭┫┃╱┃┃╰╮╭╯┃╭━━┫╭╮╭╯
        ┃╭━╮┃┃┃╰┫╰━╯┃┃╱┃┃╭╯╰╯┃╰━━┫┃╱╱┃╰━╯┃╰━╯┃╱┃┃╱┃╰━━┫┃┃╰╮
        ╰╯╱╰┻╯╰━┻━━━┻╯╱╰╯╰━━━┻━━━┻╯╱╱╰━━━┻━━━╯╱╰╯╱╰━━━┻╯╰━╯

A script to bulk download an arch linux package with all its dependencies to be converted in appimage. Add the name of a program from the Arch Linux repositories. "CHAOTIC-AUR" support can be enabled too.

------------------------------------------------------------------------
### Index
------------------------------------------------------------------------

- [History](#history)
- [Installation methods](#installation-methods)
     - [Using "AM"](#1-am-application-manager) (recommended)
     - [Using "wget"](#2-wget-the-script-directly) (locally)
     - [Using your favourite AUR helper](#3-arch-user-repository-aur)
- [Usage](#usage)
- [Related Projects](#related-projects)

--------------------------------------------------------------------

# HISTORY

This repository was archived on June 4, 2022, and reopened on July 15, 2025, for renewal and repurposing, given the continued interest.

I admit that I was inexperienced at the time and hadn't produced all the AppImage packages I have now, but I decided to reopen this repository to renew the code and improve its features where possible.

I've also worked on other packaging methods, but Arch-Deployer is an interesting project that can and will continue to improve over time, building on my current experience.

---------------------------------------------------------------------

# Installation methods

To obtain the script you can run multiple methods, the main three are:
 1. [Using "AM", the Application Manager](#1-am-application-manager) (recommended)
 2. [Using "wget"](#2-wget-the-script-directly) (locally)
 3. [Using your favourite AUR helper](#3-arch-user-repository-aur)

### 1. "AM" APPLICATION MANAGER
I recommend using "[AM" Application Manager](https://github.com/ivan-hc/AM-application-manager)", because it can easilly keep you updated with the latest version of all the programs managed, and without root permissions:
```
am -i arch-deployer
```

### 2. WGET THE SCRIPT DIRECTLY
You can obtain and run the script locally, this way:
```
wget -q https://raw.githubusercontent.com/ivan-hc/Arch-Deployer/main/arch-deployer && chmod a+x ./arch-deployer
```

### 3. ARCH USER REPOSITORY (AUR)
Using an AUR helper, for example
```
paru -S arch-deployer-git
```
NOTE: I'm not the maintainer of any AUR script.
--------------------------------------------------------------------

# USAGE:

 - `arch-deployer $PROGRAM` (download a program)
 - `arch-deployer -v` (show the version)
 - `arch-deployer -h` (show this message)

All packages are taken from https://archlinux.org/packages, AUR packages are taken from "chaotic-aur" instead, at https://builds.garudalinux.org/repos/chaotic-aur (uncomment line 7 for this)

--------------------------------------------------------------------

# RELATED PROJECTS

- **Archimage**, at https://github.com/ivan-hc/ArchImage, alternative to Arch-Deployer
- "**AM**", the package manager for AppImages and portable apps for GNU/Linux

------------------------------------------------------------------------

| [**ko-fi.com**](https://ko-fi.com/IvanAlexHC) | [**PayPal.me**](https://paypal.me/IvanAlexHC) | ["Index"](#index) |
| - | - | - |

------------------------------------------------------------------------
