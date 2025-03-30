[Back](../README.md)
# Setup PixelExperience/Any Custom Rom

## Requirements

>**PC:** 
> >Install adb

>**MOBILE:** 
> >Activate USB-Debugging
>
> >Unlock Bootloader

## Unlock Bootloader (Xiaomi-Device)

- Download Mi-Unlock-App
  - Unlock Device (if not registered, 7 days wait after register)
- Activate USB-Debugging again

## Install Recovery

>Plug the **Mobile** into the **Computer**

<hr>

>Navigate to the adb-folder &rarr; (.../adb)
- STRG + L &rarr; cmd &rarr; **'ENTER'**
    - CMD started in this folder
```
adb reboot bootloader
```
```
fastboot devices
```
(must list some ID)
```
fastboot flash recovery recovery.img
```
>Poweroff the Mobile

## Install Custom ROM

>**Start Recovery:**
> 
>Start the Mobile by Press: *Volume Up + Power*
>
> >Factory Reset &rarr; Format data/factory reset
> ><hr>
> >
> >Go Back to Main Menu
> ><hr>
> >
> >Apply Update &rarr; Apply from ADB
> > > cmd:
> > >```adb sideload rom.zip```

## Reboot Mobile and you are ready!
