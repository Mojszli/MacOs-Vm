# Disclaimer, if you see any command to run close the vm and run the cmd as admin EVERYTIME  
### And if you can undestard the process that I'm saying [this link](https://www.youtube.com/watch?v=UkdBarxP4nw) will help you out ;p

This repository is for MacOS Vm help Like iso files ect.

First you need to install [Oracle VirtualBox](https://www.virtualbox.org/wiki/Downloads) and the  
preffered iso file from either [this link](https://archive.org/details/macos_iso) or [this link](https://archive.org/details/macOS-X-images) 

Then if you have installed it dont open anything, but in the settings  
<ins>disable core isolation</ins> and <ins>disable hyper-v with this command bcdedit</ins> <ins>/set hypervisorlaunchtype off</ins>  
Please restart your computer,

Now you need to open the Vm, click on the new button
<img src="https://github.com/Mojszli/MacOs-Vm/blob/main/images/NewButton.png" alt="auto">

Then name it however you want, and select the image or iso file,  
<img src="https://github.com/Mojszli/MacOs-Vm/blob/main/images/FilledNandOS.png" alt="auto">

Allocate about 70-80 gb of storage for it,  
<img src="https://github.com/Mojszli/MacOs-Vm/blob/main/images/Storage.png" alt="auto">

Give half of your ram to it and half of your cores to it,  
<img src="https://github.com/Mojszli/MacOs-Vm/blob/main/images/Hardware.png" alt="auto">

turn off the floppy disk boot option.  
<img src="https://github.com/Mojszli/MacOs-Vm/blob/main/images/BootOption.png" alt="auto">

**If you encounter any problems contact me on dc: <ins>Mojszli</ins>**

Save it and close it and  
run these commands:

**AMD Processors**

```
 cd "C:\Program Files\Oracle\VirtualBox\"

VBoxManage.exe modifyvm "VM Name" --cpuidset 00000001 000106e5 00100800 0098e3fd bfebfbff

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "iMac19,3"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Iloveapple"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 0

VBoxManage modifyvm "VM Name" --cpu-profile "Intel Core i7-6700K"

VBoxManage setextradata "VM Name" "VBoxInternal/TM/TSCMode" "RealTSCOffset"
```

**Intel Processors**

```
 cd "C:\Program Files\Oracle\VirtualBox\"

VBoxManage.exe modifyvm "VM Name" --cpuidset 00000001 000106e5 00100800 0098e3fd bfebfbff

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "iMac19,3"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Iloveapple"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 0

VBoxManage setextradata "VM Name" "VBoxInternal/TM/TSCMode" "RealTSCOffset"
```

<ins>rename the "VM Name" to your vmbox's name</ins>

> Start the Vmbox  
> Start the Apple Virtual machine  
If your Pc freezes it will either run normal after 30 seconds or force restart your computer  
After that it will be normal  
> Complete the installation

## I will be making a a video tutorial soon..
