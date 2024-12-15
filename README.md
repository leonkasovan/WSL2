# WSL2
WSL2 Knowledge

## Prequisite:
1. Update windows 10 to 22H2
2. Activate feature: windows sub system and xxxx (i forget)

## Ubuntu 22.04 LTS
1. install from microsoft store
2. update WSL2
3. setting default for WSL2

```
sudo apt update
sudo apt upgrade
sudo apt install gcc-11 g++-11 apt-file automake autoconf libtools make cmake 
sudo apt-file update
```

## Enable GUI apps in WSL2
1. Check Windows version.  
Min required: Windows 10 version 22H2  
How to check: type `winver` in windows shell or search.

2. Update WSL  
Using Administrator In Power Shell, run this command:  
```
wsl --update
wsl --shutdown
wsl -l -v
```

## Clone WSL2 Instance (Danger, use wsl --import instead)
1. Copy source vhdx file from `C:\Users\Personal Komputer\AppData\Local\Packages\CanonicalGroupLimited.UbuntuonWindows_79rhkp1fndgsc\LocalState\ext4.vhdx`
2. Paste vhdx file into target
3. Import vhdx file `wsl --import <NewDistributionName> <InstallPath> <PathToVHDX>`
4. Example: `wsl --import Ubuntu D:\WSL\MyLinux D:\Backups\ext4.vhdx`
5. Verify `wsl --list --verbose`
6. Set default `wsl --set-version <NewDistributionName> 2`
7. 

Not Needed anymore:
```
export DISPLAY=:0.0
```
