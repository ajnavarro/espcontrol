---
title: 3.5-inch WT32-SC01 PLUS
description:
  Espcontrol on the Wireless-Tag WT32-SC01 PLUS — a 3.5-inch 320x480 portrait touchscreen with 6 cards, powered by ESP32-S3.
---

# 3.5-inch WT32-SC01 PLUS

The **Wireless-Tag WT32-SC01 PLUS** is a 3.5-inch portrait touchscreen powered by an **ESP32-S3** processor, with a 320×480 IPS display and room for **6 cards** on the home screen. It is the smallest panel Espcontrol supports and a popular choice for compact wall-mount installs.

## Specifications

| | |
|---|---|
| **Screen size** | 3.5 inches |
| **Resolution** | 320 × 480 |
| **Orientation** | Portrait |
| **Display interface** | 8-bit parallel (ST7796) |
| **Processor** | ESP32-S3 |
| **WiFi** | Built-in (2.4 GHz) |
| **Flash** | 16 MB |
| **PSRAM** | Quad, 2 MB at 80 MHz |
| **Touch** | FT6336U capacitive |
| **Power** | USB-C |

## Card Grid

The home screen uses a **3-row × 2-column** grid, giving you **6 card slots**. Any home-screen card can be turned into a [Subpage](/features/subpages) folder containing up to 5 more cards.

Flexible card sizes are supported: Single, Tall, Wide, and Large.

## Install

Connect the display to your computer with a USB-C data cable, then click the button below.

<EspInstallButton slug="wt32-sc01-plus" />

For a full walkthrough including WiFi setup and Home Assistant pairing, see the [Install guide](/getting-started/install).

## ESPHome Manual Setup

If you use ESPHome and prefer to compile firmware yourself:

```yaml
substitutions:
  name: "kitchen-screen"
  friendly_name: "Kitchen Screen"

wifi:
  ssid: !secret wifi_ssid
  password: !secret wifi_password

packages:
  setup:
    url: https://github.com/jtenniswood/espcontrol/
    file: devices/wt32-sc01-plus/packages.yaml
    refresh: 1sec
```

## Where to Buy

Sold by Wireless-Tag and various AliExpress / Amazon resellers. Search for "WT32-SC01 PLUS 3.5 inch".
