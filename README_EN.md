- [Chinese](README.md)
- [English](README_EN.md)

---
# 🛠️ ZMK Sofle Firmware Setup Guide

## 📁 Step 1: Fork the Repository

Fork the following GitHub repository:  
👉 [https://github.com/a741725193/zmk-sofle](https://github.com/a741725193/zmk-sofle)

## ⚙️ Step 2: Change the Settings

Modify the configuration as needed. For example, to decrease brightness (range 0–255):

```c
CONFIG_ZMK_RGB_UNDERGLOW_BRIGHTNESS=50
```

![image](https://github.com/user-attachments/assets/3d96b96b-4dfa-4446-831b-a27fdacf25f2)

> 🔧 Make other changes you need for your layout, behavior, or power settings.

## 💾 Step 3: Commit and Push

1. Commit your changes to your fork.
2. Push to your branch.
3. Wait for the GitHub Actions pipeline to finish building.

![image](https://github.com/user-attachments/assets/245d0fdf-4edb-46f3-865b-b1900f3162e7)

## 📦 Step 4: Download the Firmware

After the pipeline completes:

1. Download the built firmware artifacts.
2. Unzip the downloaded package.
3. You will see **3 files**, typically:

```
settings_reset-eyelash_sofle_left-zmk.uf2  
eyelash_sofle_studio_left.uf2  
nice_view_custom-eyelash_sofle_right-zmk.uf2
```
![image](https://github.com/user-attachments/assets/261de0cf-2ac6-478a-b31a-44c18a9973d8)

## 🔌 Step 5: Flash Left Half of the Keyboard

1. Connect the **left half** of the keyboard via USB.
2. Press the **reset button twice** to enter **bootloader mode**.
3. A new drive window will open.

![image](https://github.com/user-attachments/assets/a186e7cb-cf9f-48b3-b8e7-81b8eec2a85e)

### Drag & Drop Firmware Files (Left):

- First: `settings_reset-eyelash_sofle_left-zmk.uf2`  
- Wait until the drive closes.  
- Then: Press the reset button **twice again**.  
- Finally: Drag and drop `eyelash_sofle_studio_left.uf2`.

## 🔌 Step 6: Flash Right Half of the Keyboard

1. Connect the **right half** via USB.
2. Press the **reset button twice** to enter bootloader mode.
3. A new window will open.

### Drag & Drop Firmware Files (Right):

- First: `settings_reset-eyelash_sofle_left-zmk.uf2`  
- Wait until it closes.  
- Then: Press the reset button **twice again**.  
- Finally: Drag and drop `nice_view_custom-eyelash_sofle_right-zmk.uf2`.

## 🔋 Step 7: Use the Keyboard

You can now use your keyboard via:

- 🔌 USB cable (for stability and charging)
- 📶 Bluetooth (to save power)

## 🎨 Step 8: Remap Keys

Use [ZMK Studio](https://zmk.studio/) to customize key mappings.

1. Open the site.
2. Make changes visually.
3. Click **Save** to apply your new layout.

![image](https://github.com/user-attachments/assets/25d1b8b1-1d4f-4e56-9039-f824c6e22625)

<br>

# Update List

- 2024/12/21
  1. Added support for zmk-studio (just refresh the left hand to use).
- 2024/10/24
  1. Modified power supply mode to reduce power consumption.
  2. Fixed the automatic shut-off feature for RGB power supply.

> If your keyboard was updated before October 24, please update to the latest firmware.
> 

---
# Contact Me

For 3D printed model files or any issues and malfunctions with the keyboard, please contact 380465425@qq.com

# Sofle Keymap

<img src="keymap-drawer/sofle.svg" >

