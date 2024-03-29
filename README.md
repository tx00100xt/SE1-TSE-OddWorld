## Serious Sam Classic Odd World  
[![Build status](https://github.com/tx00100xt/SE1-TSE-OddWorld/actions/workflows/cibuild.yml/badge.svg)](https://github.com/tx00100xt/SE1-TSE-OddWorld/actions/)
[![License: GPL v2](https://img.shields.io/badge/License-GPL_v2-blue.svg)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html)
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/tx00100xt/SE1-TSE-OddWorld)](https://github.com/tx00100xt/SE1-TSE-OddWorld/releases/tag/v0.21)
[![Github downloads](https://img.shields.io/github/downloads/tx00100xt/SE1-TSE-OddWorld/total.svg?logo=github&logoColor=white&style=flat-square&color=E75776)](https://github.com/tx00100xt/SE1-TSE-OddWorld/releases/)

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
You can also download the archive using curl or wget:
```
wget https://archive.org/download/sam-tse-odd-world/SamTSE-OddWorld.tar.xz
```
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
After that , libraries will be collected in the Mods directory .   
Copy them to SeriousSamClassic/SamTSE/Mods/OddWorld/Bin folder.

### Ubuntu

Instead of building you can install packages from ppa by adding ppa:tx00100xt/serioussam to your system's Software Sources.
```bash
sudo add-apt-repository ppa:tx00100xt/serioussam
sudo add-apt-repository ppa:tx00100xt/serioussam-mods
sudo apt update
```
This PPA can be added to your system manually by copying the lines below and adding them to your system's software sources.
```
deb https://ppa.launchpadcontent.net/tx00100xt/serioussam/ubuntu YOUR_UBUNTU_VERSION_HERE main 
deb-src https://ppa.launchpadcontent.net/tx00100xt/serioussam/ubuntu YOUR_UBUNTU_VERSION_HERE main 
```
After adding ppa, run the commands:
```bash
sudo apt install serioussamclassic serioussamse-oddworld
```
or
```bash
sudo apt install serioussamclassic-vk serioussamse-oddworld
```

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
git clone https://github.com/tx00100xt/SE1-TSE-OddWorld.git
cd SE1-TSE-OddWorld/Sources
bash build-linux64.sh                	# use build-linux32.sh for 32-bits
```
After that , libraries will be collected in the Mods directory .   
Copy them to SeriousSamClassic/SamTSE/Mods/OddWorld/Bin folder.

### macOS

Install dependes
```
brew install bison flex sdl2 libogg libvorbis zlib-ng cmake git
```
Type this in your terminal:
```
git clone https://github.com/tx00100xt/SE1-TSE-OddWorld.git
cd SE1-TSE-OddWorld/Sources
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Release ..
make -j4
make install
```
After that , libraries will be collected in the Mods directory.   
Copy them to SeriousSamClassic/SamTSE/Mods/HNO/Bin folder.

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
* `macOS`

### Build status
|CI|Platform|Compiler|Configurations|Platforms|Status|
|---|---|---|---|---|---|
|GitHub Actions|Windows, Ubuntu, FreeBSD, Alpine, Raspberry PI OS Lite, macOS|MSVC, GCC, Clang|Release|x86, x64, armv7l, aarch64, riscv64, ppc64le, s390x|![GitHub Actions Build Status](https://github.com/tx00100xt/SE1-TSE-OddWorld/actions/workflows/cibuild.yml/badge.svg)

You can download a the automatically build based on the latest commit.  
To do this, go to the [Actions tab], select the top workflows, and then Artifacts.

License
-------

* Serious Engine v1.10 is licensed under the GNU GPL v2 (see LICENSE file).


[SamTSE-OddWorld.tar.xz]: https://drive.google.com/file/d/1nCMYxfjNeJQdaLEDDNR2DKC4sEbcoVYX/view?usp=sharing "Serious Sam Classic OddWorld Mod"
[Visual Studio 2015 Community Edition]: https://go.microsoft.com/fwlink/?LinkId=615448&clcid=0x409 "Visual Studio 2015 Community Edition"
[Windows 10 SDK 10.0.14393.795]: https://go.microsoft.com/fwlink/p/?LinkId=838916 "Windows 10 SDK 10.0.14393.795"
[Actions tab]: https://github.com/tx00100xt/SE1-TSE-OddWorld/actions "Download Artifacts"
