<p align="left"><img alt="OSPTEK" src="./images/logo.png" width="200" /></p>

<h1 align="center">OSPTEK 4.3″ TFT 480×800 (ST7102 · MIPI)</h1>

<p align="center"><b>Touch TFT module · MIPI DSI · ST7102</b></p>

<p align="center"><a href="./README.md">简体中文</a> | English · <a href="../../README_EN.md">Family index</a></p>

<p align="center">
  <img alt="Size: 4.3 inch" src="https://img.shields.io/badge/Size-4.3%22-3498DB?style=flat-square" />
  <img alt="Resolution: 480x800" src="https://img.shields.io/badge/Resolution-480%C3%97800-8E44AD?style=flat-square" />
  <img alt="Interface: MIPI" src="https://img.shields.io/badge/Interface-MIPI-27AE60?style=flat-square" />
  <img alt="Driver: ST7102" src="https://img.shields.io/badge/Driver-ST7102-E7352C?style=flat-square" />
</p>

<p align="center"><img alt="OSPTEK 4.3&quot; 480×800 TFT MIPI module (ST7102) product image" src="./images/product.png" width="640" /></p>

## Contents

- [Overview](#overview)
- [Specifications](#specifications)
- [Sample projects](#sample-projects)
- [Repository layout](#repository-layout)
- [Resources](#resources)
- [Buy](#buy)
- [Support](#support)

---

## Overview

OSPTEK **4.3″ 480×800 TFT** is a **MIPI DSI** color display module driven by **ST7102**, with touch controller **ST7123**. It suits compact HMI, handheld terminals, and portrait info panels.

Spec ID (repository name): `4.3-tft-480x800-mipi-st7102`

Current module version: **YDP430BT009-V1**. Electrical and mechanical details follow [`docs/YDP_430_BT_009_V1_a418b8470b.pdf`](./docs/YDP_430_BT_009_V1_a418b8470b.pdf).

## Specifications

| Item | Spec |
| ---- | ---- |
| Size | 4.3 inch |
| Type | TFT (color) |
| Resolution | 480×800 |
| Interface | MIPI DSI |
| Driver IC | ST7102 |
| Touch IC | ST7123 |

> Full outline, FPC definition, power, and timing follow the product datasheet / driver IC datasheet.

## Sample projects

| Description | Path |
| ---- | ---- |
| ESP32-P4 · ST7102 MIPI + esp-lvgl-port / LVGL9 | [`examples/esp32p4-idf5_st7102-mipi_esp-lvgl-port_lvgl9/`](./examples/esp32p4-idf5_st7102-mipi_esp-lvgl-port_lvgl9/) |
| ESP32-P4 · tear-related LVGL demo | [`examples/with-te/p4-idf_st7102-mipi_lvgl-common-demo/`](./examples/with-te/p4-idf_st7102-mipi_lvgl-common-demo/) |
| ESP32-P4 · ST7102 MIPI + SC2336 camera preview | [`examples/camera/esp32p4-idf5_st7102-mipi-dsi_sc2336-mipi-csi_video-lcd-display/`](./examples/camera/esp32p4-idf5_st7102-mipi-dsi_sc2336-mipi-csi_video-lcd-display/) |
| Linux · RK3566 device tree + ST7123 touch reference | [`examples/linux/`](./examples/linux/) |
| Raspberry Pi 5 · ST7102 480×800 panel / DT overlay (display only) | [`examples/rpi5-panel-st7102-480x800/`](./examples/rpi5-panel-st7102-480x800/) |
| Raspberry Pi 5 · ST7102 display + ST7123 touch / DT overlay | [`examples/rpi5-panel-st7102-st7123-480x800/`](./examples/rpi5-panel-st7102-st7123-480x800/) |

## Repository layout

```text
4.3-tft-480x800-mipi-st7102/                                # repo root (nav: ../../README_EN.md)
└── versions/
    └── YDP430BT009-V1/                                # full materials for this part number
        ├── README.md
        ├── README_EN.md
        ├── images/
        ├── docs/
        └── examples/
```

## Resources

### Product files

| Resource | Link |
| ---- | ---- |
| Product datasheet (YDP430BT009-V1) | [`docs/YDP_430_BT_009_V1_a418b8470b.pdf`](./docs/YDP_430_BT_009_V1_a418b8470b.pdf) |
| Outline drawing (YDP430BT009-V1) | [`docs/YDP430BT009-V1_外形图.pdf`](./docs/YDP430BT009-V1_%E5%A4%96%E5%BD%A2%E5%9B%BE.pdf) |
| CAD (YDP430B009-V1) | [`docs/YDP430B009-V1.dwg`](./docs/YDP430B009-V1.dwg) |
| Driver IC datasheet (ST7102) | [`docs/ST7102_Datasheet_V0.22.pdf`](./docs/ST7102_Datasheet_V0.22.pdf) |
| Init sequence (C) | [`docs/GX09C_ST7102+BOE4.3_2LANE_90HZ.c`](./docs/GX09C_ST7102+BOE4.3_2LANE_90HZ.c) |
| Timing reference (90 Hz) | [`docs/RGB_Output_Timing_90Hz.jpg`](./docs/RGB_Output_Timing_90Hz.jpg) |
| 4.3″ LCD adapter schematic | [`docs/4.3寸LCD转接板V1.0.pdf`](./docs/4.3%E5%AF%B8LCD%E8%BD%AC%E6%8E%A5%E6%9D%BFV1.0.pdf) |

### Samples

- [ESP32-P4 ST7102 MIPI + LVGL9](./examples/esp32p4-idf5_st7102-mipi_esp-lvgl-port_lvgl9/)
- [ESP32-P4 tear-related LVGL demo](./examples/with-te/p4-idf_st7102-mipi_lvgl-common-demo/)
- [ESP32-P4 ST7102 MIPI + SC2336 camera preview](./examples/camera/esp32p4-idf5_st7102-mipi-dsi_sc2336-mipi-csi_video-lcd-display/)
- [Linux RK3566 + ST7123 reference](./examples/linux/)
- [Raspberry Pi 5 ST7102 panel (display only)](./examples/rpi5-panel-st7102-480x800/)
- [Raspberry Pi 5 ST7102 display + ST7123 touch](./examples/rpi5-panel-st7102-st7123-480x800/)

## Buy

<p align="center">
  <a href="https://www.aliexpress.com/store/1105701619"><img alt="AliExpress store" src="https://img.shields.io/badge/AliExpress-Official_Store-FF6A00?style=for-the-badge" /></a>
  &nbsp;&nbsp;
  <a href="https://shop110742373.taobao.com/"><img alt="Taobao store" src="https://img.shields.io/badge/Taobao-Official_Store-FF6A00?style=for-the-badge" /></a>
</p>

**Overseas (AliExpress)**

- Store: [OSPTEK Official Store](https://www.aliexpress.com/store/1105701619)

**China (Taobao)**

- Store: [鱼鹰光电工厂店](https://shop110742373.taobao.com/)

## Support

- Technical support / product inquiry: <luyu@osptek.com>
- QQ group (China): **985881096**
- Website: <https://osptek.com/>
- Feel free to open an Issue in this repository if you have any questions

---

<p align="center"><sub>© 2026 OSPTEK · Materials in this repository are licensed under CC BY 4.0</sub></p>
