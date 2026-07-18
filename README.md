# CC-10-SRC Firmware

Official firmware for the **Transtak CC-10-SRC 10-channel relay board**.

![CC-10-SRC 10 Channels Smart Controller](cc-10-src.png)

## Download

**➡ Firmware download page: https://transtak-pte-ltd.github.io/CC-10-SRC-firmware/**

All firmware versions are also available directly on the
[Releases page](https://github.com/Transtak-Pte-Ltd/CC-10-SRC-firmware/releases).

## Flashing (ESP32)

The released `.bin` file is a **complete flash image** (bootloader + partition
table + application) and must be written to address **`0x0`**:

- **Browser (Chrome/Edge):** use the [Espressif Web Flasher](https://espressif.github.io/esptool-js/) —
  connect, choose the `.bin`, set flash address to `0x0`, program.
- **Command line:**

  ```
  pip install esptool
  esptool.py --chip esp32 --baud 921600 write_flash 0x0 smart_relay_v1.0.bin
  ```

## Configure with ThingsBoard

Video tutorial: [Smart Relay Thingsboard Configuration Tutorial](https://www.youtube.com/watch?v=RWnBdYnZ4eA)

---

© Transtak Pte Ltd
