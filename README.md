# Pixy-SM Payload Firmware
### Introduction:
  This is firmware for payload of Pixy-SM. It helps system of Pixy-SM communicate with M300 RTK and send command and adjustment to Sony A7Riv and Gimbal during operation. This firmware also collects image from sensor of Camera to live-stream on M300 RTK Remote Controller and so on.
### How to upgrade Payload Firmware with Flash Tool of Gremsy:
 #### Preparation:
  - A TYPE-C USB 
  - PC with Window OS.
  - GremsyFlashTool. Link: https://github.com/Gremsy/GremsyFlashTools_Public/releases/latest
 #### Procedure: (Detail will be mentioned in Pixy-SM manual)
  - Step 1: Connect Pixy-SM and PC with USB cable.
  - Step 2: Switch button on Pixy-SM's tilt axis to P.
  - Step 3: Hold Boot button, push Reset and Release Boot button to change Pixy-SM to BOOT MODE.
  - Step 3: Open GremsyFlashTool, choose Pixy-SM, choose "Open File", browse the path of Pixy-SM Firmware Directory (Note: Blank must not be exist)
  - Step 4: Select "Check Device".
  - Step 5: IF it notifies that "device connected. ready to flash". Chose "Flash Device" to upgrade firmware.
 
