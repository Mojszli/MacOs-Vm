# MacOs-Vm

## Disclaimer, if you see any command to run close the vm and run the cmd as admin EVERYTIME

**I will be adding pictures once i get my computer**

This repository is for MacOS Vm help Like iso files ect.

First you need to install [Oracle VirtualBox](https://www.virtualbox.org/wiki/Downloads) and the preffered iso file from either [this link](https://archive.org/details/macos_iso) or [this link](https://archive.org/details/macOS-X-images) 

Then if you have installed it dont open anything but in the settings 
disable core isolation and disable hyper-v with this command bcdedit <ins>/set hypervisorlaunchtype off</ins>
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

Save it and close it.  
Run these commands:

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


## I will be making a a video tutorial soon..
