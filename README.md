[![made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
[![built-for-android](https://forthebadge.com/images/badges/built-for-android.svg)](https://forthebadge.com)

# Android Debloater

### Clean your bloated device without root!

## Requirements

- [Android Debug Bridge](https://developer.android.com/studio/releases/platform-tools)
- [Python v3.x](https://python.org/download)
- A bloated android device

## Debloating Process

1. Clone this repo:
   ```bash
   git clone https://github.com/Kritik007/Debloat-android && cd Debloat-android
   ```
2. Connect device with `adb` and test with:
   ```bash
   adb devices
   ```
3. Run 
   ```bash
   adb shell pm list packages > pkg.list
   ```
4. Open **pkg.list** file and add a hyphen(-) to the bloat apps.
   
   For eg:
   Change
   `package:com.bloat.bs`
   to
   `-package:com.bloat.bs`

5. Save **pkg.list** and run:
   ```bash
   python debloater.py
   ```
