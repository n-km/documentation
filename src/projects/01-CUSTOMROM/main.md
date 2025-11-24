[Back](../../../README.md)
# Setup PixelExperience/Any Custom Rom

> This is a documentation of my experience using a Xiaomi Redmi Note 10 Pro

## Requirements

**PC:** 
- Install adb

**MOBILE:** 
- Activate USB-Debugging
- Unlock Bootloader

## Unlock Bootloader (Xiaomi-Device)

1. Download Mi-Unlock-App
2. Unlock Device (if not registered, there is a 7-day wait after registering)
3. Activate USB-Debugging again

## Install Recovery

**Steps:**
1. Plug the **Mobile** into the **Computer**
2. Navigate to the adb-folder (e.g., .../adb)
3. Open CMD in this folder: 
   - Press `STRG + L` 
   - Type `cmd` 
   - Press **'ENTER'**
4. Run the following commands:
    ```sh
    adb reboot bootloader
    ```
    ```
    fastboot devices
    ```
    ```
    fastboot flash recovery recovery.img
    ```
   - Ensure your device ID is listed after running `fastboot devices`
5. Power off the Mobile

## Install Custom ROM

**Steps:**
1. Start Recovery Mode:
   - Press and hold *Volume Up + Power* to start the Mobile
2. Perform a Factory Reset:
   - Navigate to: `Factory Reset` &rarr; `Format data/factory reset`
3. Apply Update:
   - Go Back to Main Menu
   - Navigate to: `Apply Update` &rarr; `Apply from ADB`
   - On your PC, run:
     ```sh
     adb sideload rom.zip
     ```

## Reboot Mobile and you are ready!
