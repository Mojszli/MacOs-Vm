# MacOs-Vm

## Disclaimer, if you see any command to run close the vm and run the cmd as admin EVERYTIME

**I will be adding pictures once i get my computer**

This repository is for MacOS Vm help Like iso files ect.

First you need to install [Oracle VirtualBox](https://www.virtualbox.org/wiki/Downloads) and the preffered iso file from either [this link](https://archive.org/details/macos_iso) or [this link](.   

Then if you have installed it dont open anything but in the settings 
disable core isolation and disable hyper-v with this command bcdedit /set hypervisorlaunchtype off
Please restart your computer,

Now you need to open the Vm, click on the new button
<img src=""alt="auto">

Then name it however you want, select the image or iso file,
allocate about 70-80 gb of storage for it, give half of your ram to it and half of your cores to it,
turn off the floppy disk boot option.

Save it and close it, for

**AMD Processors**

cd "C:\Program Files\Oracle\VirtualBox\"

VBoxManage.exe modifyvm "VM Name" --cpuidset 00000001 000106e5 00100800 0098e3fd bfebfbff

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "iMac19,3"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Iloveapple"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 0

VBoxManage modifyvm "VM Name" --cpu-profile "Intel Core i7-6700K"

VBoxManage setextradata "VM Name" "VBoxInternal/TM/TSCMode" "RealTSCOffset"


**Intel Processors**

cd "C:\Program Files\Oracle\VirtualBox\"

VBoxManage.exe modifyvm "VM Name" --cpuidset 00000001 000106e5 00100800 0098e3fd bfebfbff

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "iMac19,3"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Iloveapple"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 0

VBoxManage setextradata "VM Name" "VBoxInternal/TM/TSCMode" "RealTSCOffset"

**rename the "VM Name" to your vmbox's name**

## I will be making a a video tutorial soon..
