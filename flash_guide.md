PRE-REQUISITES:
- CLEAN FLASH: Mandatory if coming from MIUI/HyperOS 
  or any other AOSP ROM.
- DIRTY FLASH: Only supported if you are already on 
  a previous Lunaris-AOSP build.
- Remove lockscreen PIN/Password and DELETE all 
  enrolled fingerprints BEFORE flashing.

STEP 1: FLASH PARTITIONS (FASTBOOT)
(SKIP this step if you are already on an existing 
AOSP-based ROM)
fastboot flash vendor_boot vendor_boot.img
fastboot flash boot boot.img

STEP 2: FORMAT & SIDELOAD
- Reboot to Recovery (Vol Up + Power).
- FORMAT DATA: Select Factory Reset -> Format Data.
  (SKIP this only if Dirty Flashing from previous Lunaris)
- Apply Update -> Apply from ADB.
- Run: > adb sideload lunaris-aosp-v3.8.zip
- Recovery will ask: "Reboot to recovery?" -> Select YES.
- Select: Reboot System Now.

🛠️ CIT CALIBRATION (FOD & SPEAKER)
If sensors feel uncalibrated, follow this EXACTLY:
1. Phone app > Dialer > *#*#6484#*#*.
2. 3-dot menu (Top Right) > Additional Tools.
3. Select Option 5 (FOD) or Option 8 (Speaker).
4.  IMPORTANT: Once finished, REBOOT IMMEDIATELY. 
   Do not close the app or go back.
