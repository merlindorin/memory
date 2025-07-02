---
title: Flashing Raspberry Pi CM4 EEPROM with CM4-NANO-B Board
date: 2025-01-02
keywords: raspberry pi, cm4, compute module 4, eeprom, flashing, cm4-nano-b, rpiboot
---

> The CM4-NANO-B board makes flashing the Raspberry Pi Compute Module 4 EEPROM straightforward with just USB-C connection and rpiboot.

## Table of Contents
- [Problem](#problem)
- [Solution](#solution)
- [References](#references)

## Problem

Flashing the EEPROM on a Raspberry Pi Compute Module 4 (CM4) typically requires specialized hardware or complex setups. Users need a simple and reliable method to flash the CM4's eMMC storage.

## Solution

When using the CM4-NANO-B board, flashing the EEPROM becomes a simple 3-step process:

1. **Connect Power via USB-C**
   - Connect the CM4-NANO-B board to your computer using a USB-C cable
   - This connection provides both power and data link

2. **Run rpiboot**
   ```bash
   sudo ./rpiboot
   ```
   - This utility enables the CM4 to be recognized as a USB mass storage device

3. **Flash using Raspberry Pi Imager**
   - Launch Raspberry Pi Imager
   - Select your desired OS image
   - Choose the CM4 eMMC storage device (will appear after rpiboot)
   - Write the image

## References

- [How to flash Raspberry Pi OS to Compute Module 4 eMMC with usbboot - Jeff Geerling](https://www.jeffgeerling.com/blog/2020/how-flash-raspberry-pi-os-compute-module-4-emmc-usbboot)
- [CM4-NANO-B Board Specifications - Waveshare Wiki](https://www.waveshare.com/wiki/CM4-NANO-B)
- [Write Image for Compute Module Boards eMMC version - Waveshare Wiki](https://www.waveshare.com/wiki/Write_Image_for_Compute_Module_Boards_eMMC_version)