Here's the updated README file with the modified batch script code and an explanation of its components:

---

# SCRCPY Optimization Batch Script

[![Telegram Channel](https://img.shields.io/badge/Telegram-Join%20Channel-blue?style=for-the-badge&logo=telegram)](https://t.me/ping_github)

<p align="center">
  <img src="https://raw.githubusercontent.com/Genymobile/scrcpy/665ccb32f5306ebd866dc0d99f4d08ed2aeb91c3/app/data/icon.svg" alt="SCRCPY Banner" />
</p>

## Overview

This project includes a batch script for **SCRCPY** to optimize video quality, increase frame rates, and ensure smooth performance for Android screen mirroring. It’s customized for the **Xiaomi Mi 11X Pro (haydn)** but can be tailored to any Android device by adjusting the settings.

---

## Usage Instructions

1. Install **SCRCPY** from [GitHub](https://github.com/Genymobile/scrcpy).
2. Download or clone this repository.
3. Double-click the batch file `scrcpy-custom.bat` to run SCRCPY with enhanced settings.
4. You can modify the batch script according to your own device's capabilities and preferences.

### Script Example:
```batch
@echo off
:: Start SCRCPY with high-quality settings
scrcpy --video-codec=h265 --max-size=1920 --max-fps=90 --no-audio --keyboard=uhid

:: Wait for user input before closing the script
pause
```

---

## Explanation of the Script

- **`@echo off`**: This command disables the display of commands in the command prompt window, ensuring a cleaner output.

- **`scrcpy --video-codec=h265 --max-size=1920 --max-fps=90 --no-audio --keyboard=uhid`**:
   - **`--video-codec=h265`**: Sets the video codec to H.265 for better quality at lower bitrates.
   - **`--max-size=1920`**: Limits the maximum resolution of the mirrored screen to 1920 pixels wide, optimizing performance.
   - **`--max-fps=90`**: Configures the maximum frame rate to 90, providing smoother video playback.
   - **`--no-audio`**: Disables audio streaming to reduce CPU usage, focusing on video performance.
   - **`--keyboard=uhid`**: Enables the use of the USB Human Interface Device (UHID) protocol for keyboard input.

- **`pause`**: This command halts the script execution and prompts the user to press any key before closing the command prompt window. It allows the user to view any output or error messages from SCRCPY.

---

## Available Customization Options

You can tweak the batch script to fit your needs. Here are some parameters you can modify:

### 1. **Video Codec (`--video-codec`)**
   - Chooses the video encoder.
   - **Example values**: `h264`, `h265`

   ```batch
   scrcpy --video-codec=h265
   ```

### 2. **Max Resolution (`--max-size`)**
   - Sets the maximum resolution.
   - **Example values**: `1080`, `1920`

   ```batch
   scrcpy --max-size=1920
   ```

### 3. **Max FPS (`--max-fps`)**
   - Sets the frame rate cap.
   - **Example values**: `30`, `60`, `90`

   ```batch
   scrcpy --max-fps=90
   ```

### 4. **Audio Option (`--no-audio`)**
   - Disables audio streaming for performance optimization.
   - Use this option if you do not need audio.

   ```batch
   scrcpy --no-audio
   ```

### 5. **Keyboard Input (`--keyboard`)**
   - Specifies the keyboard input method.
   - Use `uhid` for USB Human Interface Device compatibility.

   ```batch
   scrcpy --keyboard=uhid
   ```

---

## Example Configurations

### High-Performance Configuration:
```batch
scrcpy --video-codec=h265 --max-size=1920 --max-fps=90 --no-audio --keyboard=uhid
```

### Low-End System Configuration:
```batch
scrcpy --video-codec=h264 --max-size=1080 --max-fps=30 --no-audio
```

---

## How to Customize

Feel free to modify any of these values directly in the `scrcpy-custom.bat` file to optimize for your specific device or computer. Refer to the [SCRCPY documentation](https://github.com/Genymobile/scrcpy) for more command options.

---

## Stay Connected

Join our Telegram community for updates, tips, and support:

[![Telegram Channel](https://img.shields.io/badge/Telegram-Join%20Channel-blue?style=for-the-badge&logo=telegram)](https://t.me/ping_github)

---

## License

This project is licensed under the MIT License.

--- 

### Summary
The README now includes a section that explains the batch script, detailing each command and its purpose, while maintaining a traditional markdown style. This helps users understand how to use the script effectively and customize it according to their needs.
