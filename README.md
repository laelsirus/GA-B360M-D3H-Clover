# GA-B360M-D3H-Clover

## Specifics

- CPU : Intel® Core™ i7-8700 Processor (12M Cache, up to 4.60 GHz)
- MAINBOARD : GIGABYTE GA-B360M D3H DURABLE EDITION
- GRAPHIC : Intel® UHD Graphics 630, SAPPAIRE RX 570 4GB
- SOUND : REALTEK ALC892
- MEMORY : ESSENCORE KLEVV DDR4 16G PC4-21300 CL16 2666MHZ (8GB * 2 DUAL CHANNEL)
- M.2 NVME SSD : SAMSUNG PM961 256GB
- 2.5 SATA SSD : SAMSUNG 960 EVO 250GB
- WIRELESS : BCM943602CS
- CASE : FRACTAL DESIGN DEFINE MINI C TEMPERED GLASS EDITION
- POWER : FSP HYPER K 600W 80PLUS STANDARD 230V EU
- COOLER : ZALMAN CNPS9X OPTIMA WHITE LED
- EXTERNAL PORT & SLOT : USB 2.0 * 2, USB 3.2 Gen 1 * 4, USB 3.2 Gen 2 * 1, TYPE C * 1 (USB 3.2 Gen 1), PS2 PORT * 1 DISPLAYPORT * 1, HDMI * 1, DVI-D * 1, D-SUB * 1, INTEL GIGABIT LAN * 1, 8CH AUDIO PORT
- DISPLAY : DELL P2417H
- SPEAKER : DELL AC511
- KEYBOARD : APPLE KEYBOARD WITH NUMERIC KEYPAD (A1243)
- MOUSE : LOGITECH T630
- WINDOWS 10 PRO


## Bios/Clover Bootloader/macOS Version

- Bios : F12
- Clover Bootloader : v2.4k r4920 (or Higher)
- macOS : Above 10.14


## Bios Setup

- Load Optimized Defaults
- [Internal Graphics] Enable


## DSDT Patch

- [sys] Add IMEI
- [sys] Fix _WAK Arg0 v2
- [sys] Fix Mutex with non-zero SyncLevel
- [sys] Fix PNOT/PPNT
- [sys] HPET Fix
- [sys] Fix IRQ Fix
- [sys] OS Check Fix (Windows 10)
- [sys] RTC Fix
- [sys] Shutdown Fix
- [sys] Shutdown Fix v2
- [sys] SMBUS Fix


## Drivers64UEFI

- ApfsDriverLoader-64.efi
- AptioMemoryFix-64.efi
- EmuVariableUefi.efi
- FSInject-64.efi
- HFSPlus.efi
- SMCHelper-64.efi


## Kexts

- AirportBrcmFixup.kext
- AppleALC.kext
- BrcmFirmwareRepo.kext
- BrcmPatchRAM2.kext
- EFICheckDisabler.kext
- FakeSMC_ACPISensors.kext
- FakeSMC_CPUSensors.kext
- FakeSMC_GPUSensors.kext
- FakeSMC_LPCSensors.kext
- FakeSMC_SMMSensors.kext
- FakeSMC.kext
- IntelMausiEthernet.kext
- Lilu.kext
- USBPorts.kext    -    Hackintool generated
- VoodooPS2Controller.kext


## ETC

***Works in headless mode***
- The output port of all internal graphics is the dummy port
If the internal graphics is not uhd 630 or if there are no external graphics, additional graphics patches might be required

***Remove these boot flags after installation***
- -v
- debug=0x100
- keepsyms=1


## Issues
none

## Screenshots

<img width="698" alt="01SystemOverview" src="https://user-images.githubusercontent.com/46496967/60285360-bf701700-9948-11e9-916b-af54a5a76fa1.png">

<img width="698" alt="02SystemDisplay" src="https://user-images.githubusercontent.com/46496967/60285249-7a4be500-9948-11e9-846b-0245575f76f0.png">

![03VideoProc](https://user-images.githubusercontent.com/46496967/60285046-07db0500-9948-11e9-801d-6a4c3945f7c3.png)

![04IntelPowerGadget](https://user-images.githubusercontent.com/46496967/60285045-07426e80-9948-11e9-95c7-a6016496a4ac.png)

![05GeekbenchCPU](https://user-images.githubusercontent.com/46496967/60285043-07426e80-9948-11e9-9290-996b3ee34ca8.png)

![06GeekbenchGPU](https://user-images.githubusercontent.com/46496967/60285041-06a9d800-9948-11e9-88de-be243d6b2dee.png)

![07USBPorts](https://user-images.githubusercontent.com/46496967/60285044-07426e80-9948-11e9-9512-bafd9b18e6ea.png)