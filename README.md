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

Not Needed anymore:
```
export DISPLAY=:0.0
```
