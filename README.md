**Hackintosh for OMEN-HP-Laptop-15-dc0xxx**

>I am not the maintainer and author of this EFI in the full sense, I just made some changes during the testing process on my machine, it is insignificant, thanks to the hard work of the original author, you can see the original author link in the README page

**❤The EFI contributor has open sourced his EFI in his GitHub Repo,you can access at the repository link below:**

https://github.com/sunmousn/OMEN-by-HP-Laptop-15-dc0xxx

---

I have returned to the Windows operating system and no longer use hackintosh. If the economic conditions are better in the future, I will consider buying Apple’s MacBook Pro 16，That will get the best experience!

**This repository is now archived**

**HP OMEN Laptop 15-dc0xxx Hackintosh OpenCore EFI**

- Original Author: MooreHarris
- Original Link: See on [PC Beta](http://bbs.pcbeta.com/forum.php?mod=viewthread&tid=1832126)
- Repair Big Sur To Work by [DejavuMoe](https://www.dejavu.moe)
- License: [MIT](https://github.com/DejavuMoe/Hackintosh-OMEN-HP-Laptop-15-dc0xxx/blob/master/LICENSE)

> 🤔 The code repository can be a bit messy, so it is recommended that you consume the [released version](https://github.com/DejavuMoe/Hackintosh-OMEN-HP-Laptop-15-dc0xxx/releases) directly.

**Configuration information**

- CPU: Intel(R) Core i5-8300H
- Integrated Graphics: Intel(R) UHD 630
- Discrete Graphics Card: Nvidia(R) Geforce GTX 1050 Ti
- Wireless Network & Bluetooth Card: Intel(R) Wireless-AC 9560AC 160 MHZ
- Sound Card: Realtek ALC 265
- Port: USB 3\*Gen3, 1\*Type-C, 1\*Rj45,1\*mini DP, 1\*HDMI

**What Works**

- CPU: Work
- Integrated Graphics: Work
- Discrete Graphics Card: Shield
- Wireless Network & Bluetooth Card: Work (See On [OpenIntelWireless](https://openintelwireless.github.io/))
- Sound Card: Work
- USB Ports: Work
- Screen Brightness Adjustment: Work
- Wake Up From Sleep: Work
- CPU Frequency Conversion: Work
- Touchpad: Work (Most gestures are available, but due to the gap between the trackpad and Mackintosh, the experience may not be increased)
- Type-C to HDMI: Work

**Test Installation Environment**

- Test System Image: Original macOS Big Sur 11.4 20F71 Installer.dmg
- System Image Writing Tool：[balenaEtcher](https://www.balena.io/etcher/)
- OpenCore Version: v0.7.0

**ScreenShots**

![](https://github.com/DejavuMoe/Hackintosh-OMEN-HP-Laptop-15-dc0xxx/blob/master/screenshots/1.png)

![](https://github.com/DejavuMoe/Hackintosh-OMEN-HP-Laptop-15-dc0xxx/blob/master/screenshots/2.png)

![](https://github.com/DejavuMoe/Hackintosh-OMEN-HP-Laptop-15-dc0xxx/blob/master/screenshots/3.png)

![](https://github.com/DejavuMoe/Hackintosh-OMEN-HP-Laptop-15-dc0xxx/blob/master/screenshots/4.png)

![](https://github.com/DejavuMoe/Hackintosh-OMEN-HP-Laptop-15-dc0xxx/blob/master/screenshots/5.png)

**File Directory Tree**

```TREE
.
|____BOOT
| |____BOOTx64.efi
| |____._BOOTx64.efi
| |____.contentFlavour
| |____._.contentFlavour
|____._BOOT
|____OC
| |____Kexts
| | |____SMCSuperIO.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____SMCSuperIO
| | | | | |____._SMCSuperIO
| | | | |____._MacOS
| | | |____._Contents
| | |____._SMCSuperIO.kext
| | |____IOElectrify.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____IOElectrify
| | | | | |____._IOElectrify
| | | | |____._MacOS
| | | |____._Contents
| | |____._IOElectrify.kext
| | |____.DS_Store
| | |____._.DS_Store
| | |____SMCLightSensor.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____SMCLightSensor
| | | | | |____._SMCLightSensor
| | | | |____._MacOS
| | | |____._Contents
| | |____._SMCLightSensor.kext
| | |____SMCProcessor.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____SMCProcessor
| | | | | |____._SMCProcessor
| | | | |____._MacOS
| | | |____._Contents
| | |____._SMCProcessor.kext
| | |____SMCBatteryManager.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____Resources
| | | | | |____SSDT-BATC.dsl
| | | | | |____._SSDT-BATC.dsl
| | | | |____._Resources
| | | | |____MacOS
| | | | | |____SMCBatteryManager
| | | | | |____._SMCBatteryManager
| | | | |____._MacOS
| | | |____._Contents
| | |____._SMCBatteryManager.kext
| | |____SMCDellSensors.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____SMCDellSensors
| | | | | |____._SMCDellSensors
| | | | |____._MacOS
| | | |____._Contents
| | |____._SMCDellSensors.kext
| | |____RealtekRTL8111.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____Resources
| | | | | |____en.lproj
| | | | | | |____InfoPlist.strings
| | | | | | |____._InfoPlist.strings
| | | | | |____._en.lproj
| | | | |____._Resources
| | | | |____MacOS
| | | | | |____RealtekRTL8111
| | | | | |____._RealtekRTL8111
| | | | |____._MacOS
| | | |____._Contents
| | |____._RealtekRTL8111.kext
| | |____IntelBluetoothFirmware.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____IntelBluetoothFirmware
| | | | | |____._IntelBluetoothFirmware
| | | | |____._MacOS
| | | |____._Contents
| | |____._IntelBluetoothFirmware.kext
| | |____ACPIBatteryManager.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____ACPIBatteryManager
| | | | | |____._ACPIBatteryManager
| | | | |____._MacOS
| | | |____._Contents
| | |____._ACPIBatteryManager.kext
| | |____AppleALC.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____AppleALC
| | | | | |____._AppleALC
| | | | |____._MacOS
| | | |____._Contents
| | |____._AppleALC.kext
| | |____AppleALCU.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____AppleALCU
| | | | | |____._AppleALCU
| | | | |____._MacOS
| | | |____._Contents
| | |____._AppleALCU.kext
| | |____AirportItlwm.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____AirportItlwm
| | | | | |____._AirportItlwm
| | | | |____._MacOS
| | | |____._Contents
| | |____._AirportItlwm.kext
| | |____VoodooPS2Controller.kext
| | | |____Contents
| | | | |____PlugIns
| | | | | |____VoodooPS2Keyboard.kext
| | | | | | |____Contents
| | | | | | | |____Info.plist
| | | | | | | |____._Info.plist
| | | | | | | |____MacOS
| | | | | | | | |____VoodooPS2Keyboard
| | | | | | | | |____._VoodooPS2Keyboard
| | | | | | | |____._MacOS
| | | | | | |____._Contents
| | | | | |____._VoodooPS2Keyboard.kext
| | | | | |____VoodooInput.kext
| | | | | | |____Contents
| | | | | | | |_____CodeSignature
| | | | | | | | |____CodeResources
| | | | | | | | |____._CodeResources
| | | | | | | |____.__CodeSignature
| | | | | | | |____Info.plist
| | | | | | | |____._Info.plist
| | | | | | | |____MacOS
| | | | | | | | |____VoodooInput
| | | | | | | | |____._VoodooInput
| | | | | | | |____._MacOS
| | | | | | |____._Contents
| | | | | |____._VoodooInput.kext
| | | | | |____VoodooPS2Trackpad.kext
| | | | | | |____Contents
| | | | | | | |____Info.plist
| | | | | | | |____._Info.plist
| | | | | | | |____MacOS
| | | | | | | | |____VoodooPS2Trackpad
| | | | | | | | |____._VoodooPS2Trackpad
| | | | | | | |____._MacOS
| | | | | | |____._Contents
| | | | | |____._VoodooPS2Trackpad.kext
| | | | | |____VoodooPS2Mouse.kext
| | | | | | |____Contents
| | | | | | | |____Info.plist
| | | | | | | |____._Info.plist
| | | | | | | |____MacOS
| | | | | | | | |____VoodooPS2Mouse
| | | | | | | | |____._VoodooPS2Mouse
| | | | | | | |____._MacOS
| | | | | | |____._Contents
| | | | | |____._VoodooPS2Mouse.kext
| | | | |____._PlugIns
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____VoodooPS2Controller
| | | | | |____._VoodooPS2Controller
| | | | |____._MacOS
| | | |____._Contents
| | |____._VoodooPS2Controller.kext
| | |____CtlnaAHCIPort.kext
| | | |____Contents
| | | | |_____CodeSignature
| | | | | |____CodeResources
| | | | | |____._CodeResources
| | | | |____.__CodeSignature
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____CtlnaAHCIPort
| | | | | |____._CtlnaAHCIPort
| | | | |____._MacOS
| | | | |____version.plist
| | | | |____._version.plist
| | | |____._Contents
| | |____._CtlnaAHCIPort.kext
| | |____IntelBluetoothInjector.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | |____._Contents
| | |____._IntelBluetoothInjector.kext
| | |____USBPorts.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | |____._Contents
| | |____._USBPorts.kext
| | |____VirtualSMC.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____VirtualSMC
| | | | | |____._VirtualSMC
| | | | |____._MacOS
| | | |____._Contents
| | |____._VirtualSMC.kext
| | |____WhateverGreen.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____WhateverGreen
| | | | | |____._WhateverGreen
| | | | |____._MacOS
| | | |____._Contents
| | |____._WhateverGreen.kext
| | |____ApplePS2SmartTouchPad.kext
| | | |____Contents
| | | | |____PlugIns
| | | | | |____ApplePS2Controller.kext
| | | | | | |____Contents
| | | | | | | |____Info.plist
| | | | | | | |____._Info.plist
| | | | | | | |____MacOS
| | | | | | | | |____ApplePS2Controller
| | | | | | | | |____._ApplePS2Controller
| | | | | | | |____._MacOS
| | | | | | |____._Contents
| | | | | |____._ApplePS2Controller.kext
| | | | | |____ApplePS2Keyboard.kext
| | | | | | |____Contents
| | | | | | | |____Info.plist
| | | | | | | |____._Info.plist
| | | | | | | |____MacOS
| | | | | | | | |____ApplePS2Keyboard
| | | | | | | | |____._ApplePS2Keyboard
| | | | | | | |____._MacOS
| | | | | | |____._Contents
| | | | | |____._ApplePS2Keyboard.kext
| | | | |____._PlugIns
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____Resources
| | | | | |____Synaptics documentation.rtfd
| | | | | | |____page42image78240.png
| | | | | | |____._page42image78240.png
| | | | | | |____page42image105384.png
| | | | | | |____._page42image105384.png
| | | | | | |____page43image48560.png
| | | | | | |____._page43image48560.png
| | | | | | |____page30image68112.png
| | | | | | |____._page30image68112.png
| | | | | | |____page30image45080.png
| | | | | | |____._page30image45080.png
| | | | | | |____page30image42512.png
| | | | | | |____._page30image42512.png
| | | | | | |____page43image25376.png
| | | | | | |____._page43image25376.png
| | | | | | |____page42image77600.png
| | | | | | |____._page42image77600.png
| | | | | | |____page42image78848.png
| | | | | | |____._page42image78848.png
| | | | | | |____page30image64064.png
| | | | | | |____._page30image64064.png
| | | | | | |____page30image48000.png
| | | | | | |____._page30image48000.png
| | | | | | |____page42image97536.png
| | | | | | |____._page42image97536.png
| | | | | | |____page30image67632.png
| | | | | | |____._page30image67632.png
| | | | | | |____page30image39000.png
| | | | | | |____._page30image39000.png
| | | | | | |____page30image21840.png
| | | | | | |____._page30image21840.png
| | | | | | |____page30image28496.png
| | | | | | |____._page30image28496.png
| | | | | | |____page30image66064.png
| | | | | | |____._page30image66064.png
| | | | | | |____page43image34240.png
| | | | | | |____._page43image34240.png
| | | | | | |____page30image35992.png
| | | | | | |____._page30image35992.png
| | | | | | |____page43image36720.png
| | | | | | |____._page43image36720.png
| | | | | | |____page30image65424.png
| | | | | | |____._page30image65424.png
| | | | | | |____page43image29984.png
| | | | | | |____._page43image29984.png
| | | | | | |____page30image64672.png
| | | | | | |____._page30image64672.png
| | | | | | |____page30image26496.png
| | | | | | |____._page30image26496.png
| | | | | | |____page30image38680.png
| | | | | | |____._page30image38680.png
| | | | | | |____page30image45872.png
| | | | | | |____._page30image45872.png
| | | | | | |____page30image65744.png
| | | | | | |____._page30image65744.png
| | | | | | |____page30image33264.png
| | | | | | |____._page30image33264.png
| | | | | | |____page43image35968.png
| | | | | | |____._page43image35968.png
| | | | | | |____page30image31936.png
| | | | | | |____._page30image31936.png
| | | | | | |____page43image30408.png
| | | | | | |____._page43image30408.png
| | | | | | |____page30image68856.png
| | | | | | |____._page30image68856.png
| | | | | | |____page42image75600.png
| | | | | | |____._page42image75600.png
| | | | | | |____page42image99496.png
| | | | | | |____._page42image99496.png
| | | | | | |____page30image16608.png
| | | | | | |____._page30image16608.png
| | | | | | |____page42image76080.png
| | | | | | |____._page42image76080.png
| | | | | | |____page30image62200.png
| | | | | | |____._page30image62200.png
| | | | | | |____page42image95864.png
| | | | | | |____._page42image95864.png
| | | | | | |____page42image75760.png
| | | | | | |____._page42image75760.png
| | | | | | |____page30image37272.png
| | | | | | |____._page30image37272.png
| | | | | | |____page30image32256.png
| | | | | | |____._page30image32256.png
| | | | | | |____page30image34168.png
| | | | | | |____._page30image34168.png
| | | | | | |____page30image31776.png
| | | | | | |____._page30image31776.png
| | | | | | |____page30image18496.png
| | | | | | |____._page30image18496.png
| | | | | | |____page42image86936.png
| | | | | | |____._page42image86936.png
| | | | | | |____page30image32096.png
| | | | | | |____._page30image32096.png
| | | | | | |____page43image35648.png
| | | | | | |____._page43image35648.png
| | | | | | |____page30image35672.png
| | | | | | |____._page30image35672.png
| | | | | | |____page43image32696.png
| | | | | | |____._page43image32696.png
| | | | | | |____page30image65904.png
| | | | | | |____._page30image65904.png
| | | | | | |____page30image57008.png
| | | | | | |____._page30image57008.png
| | | | | | |____page42image88112.png
| | | | | | |____._page42image88112.png
| | | | | | |____page30image31616.png
| | | | | | |____._page30image31616.png
| | | | | | |____page30image64832.png
| | | | | | |____._page30image64832.png
| | | | | | |____page43image31160.png
| | | | | | |____._page43image31160.png
| | | | | | |____page43image24784.png
| | | | | | |____._page43image24784.png
| | | | | | |____page43image26144.png
| | | | | | |____._page43image26144.png
| | | | | | |____page42image93040.png
| | | | | | |____._page42image93040.png
| | | | | | |____page42image88272.png
| | | | | | |____._page42image88272.png
| | | | | | |____page30image37112.png
| | | | | | |____._page30image37112.png
| | | | | | |____page30image47224.png
| | | | | | |____._page30image47224.png
| | | | | | |____page30image60112.png
| | | | | | |____._page30image60112.png
| | | | | | |____page30image25248.png
| | | | | | |____._page30image25248.png
| | | | | | |____page30image59368.png
| | | | | | |____._page30image59368.png
| | | | | | |____page30image63744.png
| | | | | | |____._page30image63744.png
| | | | | | |____page30image36792.png
| | | | | | |____._page30image36792.png
| | | | | | |____page30image25088.png
| | | | | | |____._page30image25088.png
| | | | | | |____page30image40360.png
| | | | | | |____._page30image40360.png
| | | | | | |____page43image30736.png
| | | | | | |____._page43image30736.png
| | | | | | |____page30image44072.png
| | | | | | |____._page30image44072.png
| | | | | | |____page43image53736.png
| | | | | | |____._page43image53736.png
| | | | | | |____page30image29088.png
| | | | | | |____._page30image29088.png
| | | | | | |____page43image26624.png
| | | | | | |____._page43image26624.png
| | | | | | |____page30image63424.png
| | | | | | |____._page30image63424.png
| | | | | | |____page42image79272.png
| | | | | | |____._page42image79272.png
| | | | | | |____page42image77920.png
| | | | | | |____._page42image77920.png
| | | | | | |____page30image60272.png
| | | | | | |____._page30image60272.png
| | | | | | |____page30image15160.png
| | | | | | |____._page30image15160.png
| | | | | | |____page30image42992.png
| | | | | | |____._page30image42992.png
| | | | | | |____page30image24168.png
| | | | | | |____._page30image24168.png
| | | | | | |____page43image28152.png
| | | | | | |____._page43image28152.png
| | | | | | |____page30image58464.png
| | | | | | |____._page30image58464.png
| | | | | | |____page30image36632.png
| | | | | | |____._page30image36632.png
| | | | | | |____page30image56688.png
| | | | | | |____._page30image56688.png
| | | | | | |____page43image33392.png
| | | | | | |____._page43image33392.png
| | | | | | |____page42image87360.png
| | | | | | |____._page42image87360.png
| | | | | | |____page42image88912.png
| | | | | | |____._page42image88912.png
| | | | | | |____page43image46136.png
| | | | | | |____._page43image46136.png
| | | | | | |____page42image77440.png
| | | | | | |____._page42image77440.png
| | | | | | |____page30image56848.png
| | | | | | |____._page30image56848.png
| | | | | | |____page43image54056.png
| | | | | | |____._page43image54056.png
| | | | | | |____page30image50744.png
| | | | | | |____._page30image50744.png
| | | | | | |____page43image33232.png
| | | | | | |____._page43image33232.png
| | | | | | |____page43image26944.png
| | | | | | |____._page43image26944.png
| | | | | | |____page30image35080.png
| | | | | | |____._page30image35080.png
| | | | | | |____page30image13912.png
| | | | | | |____._page30image13912.png
| | | | | | |____TXT.rtf
| | | | | | |____._TXT.rtf
| | | | | | |____page30image20328.png
| | | | | | |____._page30image20328.png
| | | | | | |____page30image54640.png
| | | | | | |____._page30image54640.png
| | | | | | |____page30image36952.png
| | | | | | |____._page30image36952.png
| | | | | | |____page30image41264.png
| | | | | | |____._page30image41264.png
| | | | | | |____page42image76832.png
| | | | | | |____._page42image76832.png
| | | | | | |____page42image84520.png
| | | | | | |____._page42image84520.png
| | | | | | |____page42image82192.png
| | | | | | |____._page42image82192.png
| | | | | | |____page30image67472.png
| | | | | | |____._page30image67472.png
| | | | | | |____page30image53728.png
| | | | | | |____._page30image53728.png
| | | | | | |____page30image66224.png
| | | | | | |____._page30image66224.png
| | | | | | |____page43image52024.png
| | | | | | |____._page43image52024.png
| | | | | | |____page42image81272.png
| | | | | | |____._page42image81272.png
| | | | | | |____page30image26984.png
| | | | | | |____._page30image26984.png
| | | | | | |____page30image49832.png
| | | | | | |____._page30image49832.png
| | | | | | |____page30image68432.png
| | | | | | |____._page30image68432.png
| | | | | | |____page30image54320.png
| | | | | | |____._page30image54320.png
| | | | | | |____page43image37520.png
| | | | | | |____._page43image37520.png
| | | | | | |____page42image86456.png
| | | | | | |____._page42image86456.png
| | | | | | |____page43image25536.png
| | | | | | |____._page43image25536.png
| | | | | | |____page43image51704.png
| | | | | | |____._page43image51704.png
| | | | | | |____page30image16448.png
| | | | | | |____._page30image16448.png
| | | | | | |____page43image33816.png
| | | | | | |____._page43image33816.png
| | | | | | |____page30image62040.png
| | | | | | |____._page30image62040.png
| | | | | | |____page30image14840.png
| | | | | | |____._page30image14840.png
| | | | | | |____page43image48136.png
| | | | | | |____._page43image48136.png
| | | | | | |____page30image45400.png
| | | | | | |____._page30image45400.png
| | | | | | |____page30image67312.png
| | | | | | |____._page30image67312.png
| | | | | | |____page30image49992.png
| | | | | | |____._page30image49992.png
| | | | | | |____page30image52480.png
| | | | | | |____._page30image52480.png
| | | | | | |____page42image83992.png
| | | | | | |____._page42image83992.png
| | | | | | |____page30image60432.png
| | | | | | |____._page30image60432.png
| | | | | | |____page43image54544.png
| | | | | | |____._page43image54544.png
| | | | | | |____page43image50440.png
| | | | | | |____._page43image50440.png
| | | | | | |____page30image61880.png
| | | | | | |____._page30image61880.png
| | | | | | |____page43image24464.png
| | | | | | |____._page43image24464.png
| | | | | | |____page42image103272.png
| | | | | | |____._page42image103272.png
| | | | | | |____page42image85528.png
| | | | | | |____._page42image85528.png
| | | | | | |____page30image57328.png
| | | | | | |____._page30image57328.png
| | | | | | |____page30image34328.png
| | | | | | |____._page30image34328.png
| | | | | | |____page42image85104.png
| | | | | | |____._page42image85104.png
| | | | | | |____page30image31456.png
| | | | | | |____._page30image31456.png
| | | | | | |____page43image27568.png
| | | | | | |____._page43image27568.png
| | | | | | |____page30image63104.png
| | | | | | |____._page30image63104.png
| | | | | | |____page43image26304.png
| | | | | | |____._page43image26304.png
| | | | | | |____page43image55936.png
| | | | | | |____._page43image55936.png
| | | | | | |____page30image33848.png
| | | | | | |____._page30image33848.png
| | | | | | |____page30image36312.png
| | | | | | |____._page30image36312.png
| | | | | | |____page42image96184.png
| | | | | | |____._page42image96184.png
| | | | | | |____page43image36880.png
| | | | | | |____._page43image36880.png
| | | | | | |____page30image34920.png
| | | | | | |____._page30image34920.png
| | | | | | |____page30image59528.png
| | | | | | |____._page30image59528.png
| | | | | | |____page30image59048.png
| | | | | | |____._page30image59048.png
| | | | | | |____page42image76672.png
| | | | | | |____._page42image76672.png
| | | | | | |____page30image51992.png
| | | | | | |____._page30image51992.png
| | | | | | |____page43image24304.png
| | | | | | |____._page43image24304.png
| | | | | | |____page30image22000.png
| | | | | | |____._page30image22000.png
| | | | | | |____page30image47840.png
| | | | | | |____._page30image47840.png
| | | | | | |____page30image18808.png
| | | | | | |____._page30image18808.png
| | | | | | |____page30image13008.png
| | | | | | |____._page30image13008.png
| | | | | | |____page30image13432.png
| | | | | | |____._page30image13432.png
| | | | | | |____page43image49048.png
| | | | | | |____._page43image49048.png
| | | | | | |____page43image35168.png
| | | | | | |____._page43image35168.png
| | | | | | |____page30image57648.png
| | | | | | |____._page30image57648.png
| | | | | | |____page42image105808.png
| | | | | | |____._page42image105808.png
| | | | | | |____page30image44392.png
| | | | | | |____._page30image44392.png
| | | | | | |____page30image57488.png
| | | | | | |____._page30image57488.png
| | | | | | |____page30image24328.png
| | | | | | |____._page30image24328.png
| | | | | | |____page30image69176.png
| | | | | | |____._page30image69176.png
| | | | | | |____page30image36472.png
| | | | | | |____._page30image36472.png
| | | | | | |____page30image32416.png
| | | | | | |____._page30image32416.png
| | | | | |____._Synaptics documentation.rtfd
| | | | | |____Features Documentation.rtfd
| | | | | | |____9718452526_b6414cd8e7_n.jpg
| | | | | | |____._9718452526_b6414cd8e7_n.jpg
| | | | | | |____11493706554_130fa58d5f_n.jpg
| | | | | | |____._11493706554_130fa58d5f_n.jpg
| | | | | | |____TXT.rtf
| | | | | | |____._TXT.rtf
| | | | | | |____8524384148_7da070dae6_c.jpg
| | | | | | |____._8524384148_7da070dae6_c.jpg
| | | | | |____._Features Documentation.rtfd
| | | | |____._Resources
| | | | |____MacOS
| | | | | |____ApplePS2SmartTouchPad
| | | | | |____._ApplePS2SmartTouchPad
| | | | |____._MacOS
| | | |____._Contents
| | |____._ApplePS2SmartTouchPad.kext
| | |____HibernationFixup.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____HibernationFixup
| | | | | |____._HibernationFixup
| | | | |____._MacOS
| | | |____._Contents
| | |____._HibernationFixup.kext
| | |____NVMeFix.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____NVMeFix
| | | | | |____._NVMeFix
| | | | |____._MacOS
| | | |____._Contents
| | |____._NVMeFix.kext
| | |____Lilu.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____Lilu
| | | | | |____._Lilu
| | | | |____._MacOS
| | | |____._Contents
| | |____._Lilu.kext
| | |____RTCMemoryFixup.kext
| | | |____Contents
| | | | |____Info.plist
| | | | |____._Info.plist
| | | | |____MacOS
| | | | | |____RTCMemoryFixup
| | | | | |____._RTCMemoryFixup
| | | | |____._MacOS
| | | |____._Contents
| | |____._RTCMemoryFixup.kext
| |____._Kexts
| |____.DS_Store
| |____._.DS_Store
| |____Drivers
| | |____OpenRuntime.efi
| | |____._OpenRuntime.efi
| | |____.DS_Store
| | |____._.DS_Store
| | |____OpenHfsPlus.efi
| | |____._OpenHfsPlus.efi
| | |____OpenCanopy.efi
| | |____._OpenCanopy.efi
| |____._Drivers
| |____Tools
| | |____CsrUtil.efi
| | |____._CsrUtil.efi
| | |____ResetSystem.efi
| | |____._ResetSystem.efi
| | |____OpenControl.efi
| | |____._OpenControl.efi
| | |____RtcRw.efi
| | |____._RtcRw.efi
| | |____MmapDump.efi
| | |____._MmapDump.efi
| | |____ControlMsrE2.efi
| | |____._ControlMsrE2.efi
| | |____ChipTune.efi
| | |____._ChipTune.efi
| | |____OpenShell.efi
| | |____._OpenShell.efi
| | |____KeyTester.efi
| | |____._KeyTester.efi
| | |____GopStop.efi
| | |____._GopStop.efi
| | |____BootKicker.efi
| | |____._BootKicker.efi
| | |____CleanNvram.efi
| | |____._CleanNvram.efi
| |____._Tools
| |____.contentFlavour
| |____._.contentFlavour
| |____OpenCore.efi
| |____._OpenCore.efi
| |____Resources
| | |____.DS_Store
| | |____._.DS_Store
| | |____Image
| | | |____Acidanthera
| | | | |____Chardonnay
| | | | | |____Left.icns
| | | | | |____._Left.icns
| | | | | |____Password.icns
| | | | | |____._Password.icns
| | | | | |____ExtHardDrive.icns
| | | | | |____._ExtHardDrive.icns
| | | | | |____Tool.icns
| | | | | |____._Tool.icns
| | | | | |____HardDrive.icns
| | | | | |____._HardDrive.icns
| | | | | |____Shell.icns
| | | | | |____._Shell.icns
| | | | | |____Selector.icns
| | | | | |____._Selector.icns
| | | | | |____Restart.icns
| | | | | |____._Restart.icns
| | | | | |____Right.icns
| | | | | |____._Right.icns
| | | | | |____Selected.icns
| | | | | |____._Selected.icns
| | | | | |____Enter.icns
| | | | | |____._Enter.icns
| | | | | |____Windows.icns
| | | | | |____._Windows.icns
| | | | | |____Lock.icns
| | | | | |____._Lock.icns
| | | | | |____Cursor.icns
| | | | | |____._Cursor.icns
| | | | | |____SetDefault.icns
| | | | | |____._SetDefault.icns
| | | | | |____AppleTM.icns
| | | | | |____._AppleTM.icns
| | | | | |____BtnFocus.icns
| | | | | |____._BtnFocus.icns
| | | | | |____AppleRecv.icns
| | | | | |____._AppleRecv.icns
| | | | | |____Dot.icns
| | | | | |____._Dot.icns
| | | | | |____ShutDown.icns
| | | | | |____._ShutDown.icns
| | | | | |____ExtAppleTM.icns
| | | | | |____._ExtAppleTM.icns
| | | | | |____ExtAppleRecv.icns
| | | | | |____._ExtAppleRecv.icns
| | | | |____._Chardonnay
| | | | |____Syrah
| | | | | |____Left.icns
| | | | | |____._Left.icns
| | | | | |____Password.icns
| | | | | |____._Password.icns
| | | | | |____ExtHardDrive.icns
| | | | | |____._ExtHardDrive.icns
| | | | | |____Tool.icns
| | | | | |____._Tool.icns
| | | | | |____HardDrive.icns
| | | | | |____._HardDrive.icns
| | | | | |____Shell.icns
| | | | | |____._Shell.icns
| | | | | |____Selector.icns
| | | | | |____._Selector.icns
| | | | | |____Restart.icns
| | | | | |____._Restart.icns
| | | | | |____Right.icns
| | | | | |____._Right.icns
| | | | | |____Selected.icns
| | | | | |____._Selected.icns
| | | | | |____Enter.icns
| | | | | |____._Enter.icns
| | | | | |____Windows.icns
| | | | | |____._Windows.icns
| | | | | |____Lock.icns
| | | | | |____._Lock.icns
| | | | | |____Cursor.icns
| | | | | |____._Cursor.icns
| | | | | |____SetDefault.icns
| | | | | |____._SetDefault.icns
| | | | | |____AppleTM.icns
| | | | | |____._AppleTM.icns
| | | | | |____BtnFocus.icns
| | | | | |____._BtnFocus.icns
| | | | | |____AppleRecv.icns
| | | | | |____._AppleRecv.icns
| | | | | |____Dot.icns
| | | | | |____._Dot.icns
| | | | | |____ShutDown.icns
| | | | | |____._ShutDown.icns
| | | | | |____ExtAppleTM.icns
| | | | | |____._ExtAppleTM.icns
| | | | | |____ExtAppleRecv.icns
| | | | | |____._ExtAppleRecv.icns
| | | | |____._Syrah
| | | | |____GoldenGate
| | | | | |____Left.icns
| | | | | |____._Left.icns
| | | | | |____Password.icns
| | | | | |____._Password.icns
| | | | | |____ExtHardDrive.icns
| | | | | |____._ExtHardDrive.icns
| | | | | |____Tool.icns
| | | | | |____._Tool.icns
| | | | | |____HardDrive.icns
| | | | | |____._HardDrive.icns
| | | | | |____Shell.icns
| | | | | |____._Shell.icns
| | | | | |____Selector.icns
| | | | | |____._Selector.icns
| | | | | |____Restart.icns
| | | | | |____._Restart.icns
| | | | | |____Right.icns
| | | | | |____._Right.icns
| | | | | |____Selected.icns
| | | | | |____._Selected.icns
| | | | | |____Enter.icns
| | | | | |____._Enter.icns
| | | | | |____Windows.icns
| | | | | |____._Windows.icns
| | | | | |____Lock.icns
| | | | | |____._Lock.icns
| | | | | |____Cursor.icns
| | | | | |____._Cursor.icns
| | | | | |____SetDefault.icns
| | | | | |____._SetDefault.icns
| | | | | |____AppleTM.icns
| | | | | |____._AppleTM.icns
| | | | | |____BtnFocus.icns
| | | | | |____._BtnFocus.icns
| | | | | |____AppleRecv.icns
| | | | | |____._AppleRecv.icns
| | | | | |____Dot.icns
| | | | | |____._Dot.icns
| | | | | |____ShutDown.icns
| | | | | |____._ShutDown.icns
| | | | | |____ExtAppleTM.icns
| | | | | |____._ExtAppleTM.icns
| | | | | |____ExtAppleRecv.icns
| | | | | |____._ExtAppleRecv.icns
| | | | |____._GoldenGate
| | | |____._Acidanthera
| | |____._Image
| | |____Label
| | | |____Windows.lbl
| | | |____._Windows.lbl
| | | |____Shell.l2x
| | | |____._Shell.l2x
| | | |____SIPEnabled.l2x
| | | |____._SIPEnabled.l2x
| | | |____AppleTM.l2x
| | | |____._AppleTM.l2x
| | | |____Tool.lbl
| | | |____._Tool.lbl
| | | |____Apple.lbl
| | | |____._Apple.lbl
| | | |____EFIBoot.l2x
| | | |____._EFIBoot.l2x
| | | |____Other.lbl
| | | |____._Other.lbl
| | | |____SIPDisabled.l2x
| | | |____._SIPDisabled.l2x
| | | |____AppleRecv.lbl
| | | |____._AppleRecv.lbl
| | | |____ResetNVRAM.lbl
| | | |____._ResetNVRAM.lbl
| | | |____Tool.l2x
| | | |____._Tool.l2x
| | | |____Apple.l2x
| | | |____._Apple.l2x
| | | |____EFIBoot.lbl
| | | |____._EFIBoot.lbl
| | | |____SIPDisabled.lbl
| | | |____._SIPDisabled.lbl
| | | |____Other.l2x
| | | |____._Other.l2x
| | | |____AppleRecv.l2x
| | | |____._AppleRecv.l2x
| | | |____ResetNVRAM.l2x
| | | |____._ResetNVRAM.l2x
| | | |____Windows.l2x
| | | |____._Windows.l2x
| | | |____Shell.lbl
| | | |____._Shell.lbl
| | | |____SIPEnabled.lbl
| | | |____._SIPEnabled.lbl
| | | |____AppleTM.lbl
| | | |____._AppleTM.lbl
| | |____._Label
| | |____Font
| | | |____Font_1x.bin
| | | |____._Font_1x.bin
| | | |____Font_1x.png
| | | |____._Font_1x.png
| | | |____Font_2x.png
| | | |____._Font_2x.png
| | | |____Font_2x.bin
| | | |____._Font_2x.bin
| | |____._Font
| |____._Resources
| |____ACPI
| | |____SSDT-SMBUS.aml
| | |____._SSDT-SMBUS.aml
| | |____SSDT-DGPU.aml
| | |____._SSDT-DGPU.aml
| | |____SSDT-PMC.aml
| | |____._SSDT-PMC.aml
| | |____DSDT-FN F4 Keyboard light.aml
| | |____._DSDT-FN F4 Keyboard light.aml
| | |____SSDT-AWAC-DISABLE.aml
| | |____._SSDT-AWAC-DISABLE.aml
| | |____SSDT-EC.aml
| | |____._SSDT-EC.aml
| | |____SSDT-XOSI.aml
| | |____._SSDT-XOSI.aml
| | |____SSDT-XCPM.aml
| | |____._SSDT-XCPM.aml
| | |____DSDT.aml
| | |____._DSDT.aml
| | |____SSDT-PNLFCFL.aml
| | |____._SSDT-PNLFCFL.aml
| |____._ACPI
| |____._config.plist
| |____config.plist
|____._OC
```

