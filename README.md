## Serious Sam Classic Odd World

What is Odd World?  
This is a modification for Serious Sam Classic The Second Encounter.  
This mod required https://github.com/tx00100xt/SeriousSamClassic or https://github.com/tx00100xt/SeriousSamClassic-VK to run.  
Odd World was created by fans of the game Serious Sam Classic and is distributed for free.    

Description:  
Faster than a speeding werebull!
Leap over walls in a single bound!  
Its a bird! Its a plane! No! Its Sam-Da-Man! He's back and ready to kick some more ass in this high adrenaline modification.
OddWorld takes you through the same great game but its faster, more action packed, and will blow you away (quite literally).
Don't be the last one to get this great mod!    

Author:  
Louva-Deus is author this mod for windows.  

![OW1](https://raw.githubusercontent.com/tx00100xt/SE1-TSE-OddWorld/main/Images/oddworld-1.png)

![OW2](https://raw.githubusercontent.com/tx00100xt/SE1-TSE-OddWorld/main/Images/oddworld-2.png)


Download [SamTSE-OddWorld.tar.xz] archive and unpack to  SeriousSamClassic/SamTSE/ directory.  
To start the modification, use the game menu - item Modification.

Building Serious Sam Classic Odd World modification (only for SS:TSE)
---------------------------------------------------------------------

### Linux

Type this in your terminal:

```
git clone https://github.com/tx00100xt/SE1-TSE-OddWorld.git SE1-TSE-OddWorld
cd SE1-TSE-OddWorld/Sources
./build-linux64.sh                  	# use build-linux32.sh for 32-bits
```
After that , libraries will be collected in the x32 or x64 directory .   
Copy them to SeriousSamClassic/SamTSE/Mods/OddWorld/Bin folder.

### Gentoo

To build a game for gentoo, use a https://github.com/tx00100xt/serioussam-overlay containing ready-made ebuilds for building the game and add-ons.

### Arch Linux

To build a game under Arch Linux you can use the package from AUR: https://aur.archlinux.org/packages/serioussam

### Raspberry Pi

The build for raspberry pi is similar to the build for Linux, you just need to add an additional build key.

```
cd SE1-TSE-OddWorld/Sources
./build-linux64.sh -DRPI4=TRUE	        # use build-linux32.sh for 32-bits
```
### FreeBSD

Install bash. 
Type this in your terminal:

```
git clone https://github.com/tx00100xt/SE1-TSE-OddWorld.git SE1-TSE-OddWorld
cd SE1-TSE-OddWorld/Sources
bash build-linux64.sh                	# use build-linux32.sh for 32-bits
```
After that , libraries will be collected in the x32 or x64 directory .   
Copy them to SeriousSamClassic/SamTSE/Mods/OddWorld/Bin folder.

Windows
-------
* This project can be compiled starting from Windows 7 and higher.

1. Download and Install [Visual Studio 2015 Community Edition] or higher.
2. Download and Install [Windows 10 SDK 10.0.14393.795] or other.
3. Open the solution in the Sources folder, select Release x64 or Release Win32 and compile it.

Supported Architectures
----------------------
* `x86`
* `aarch64`
* `e2k` (elbrus)

Supported OS
-----------
* `Linux`
* `FreeBSD`
* `Windows`
* `Raspberry PI OS`

License
-------

* Serious Engine v1.10 is licensed under the GNU GPL v2 (see LICENSE file).


[SamTSE-OddWorld.tar.xz]: https://drive.google.com/file/d/1nCMYxfjNeJQdaLEDDNR2DKC4sEbcoVYX/view?usp=sharing "Serious Sam Classic OddWorld Mod"
[Visual Studio 2015 Community Edition]: https://go.microsoft.com/fwlink/?LinkId=615448&clcid=0x409 "Visual Studio 2015 Community Edition"
[Windows 10 SDK 10.0.14393.795]: https://go.microsoft.com/fwlink/p/?LinkId=838916 "Windows 10 SDK 10.0.14393.795"
