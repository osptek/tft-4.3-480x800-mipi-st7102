<p align="left"><img alt="OSPTEK" src="./images/logo.png" width="200" /></p>

<h1 align="center">OSPTEK 4.3″ TFT 480×800（ST7102 · MIPI）</h1>

<p align="center"><b>触摸 TFT 模组 · MIPI DSI · ST7102</b></p>

<p align="center"><a href="./README_EN.md">English</a> | 简体中文 · <a href="../../README.md">规格族索引</a></p>

<p align="center">
  <img alt="Size: 4.3 inch" src="https://img.shields.io/badge/Size-4.3%22-3498DB?style=flat-square" />
  <img alt="Resolution: 480x800" src="https://img.shields.io/badge/Resolution-480%C3%97800-8E44AD?style=flat-square" />
  <img alt="Interface: MIPI" src="https://img.shields.io/badge/Interface-MIPI-27AE60?style=flat-square" />
  <img alt="Driver: ST7102" src="https://img.shields.io/badge/Driver-ST7102-E7352C?style=flat-square" />
</p>

<p align="center"><img alt="OSPTEK 4.3 寸 480×800 TFT MIPI 模组（ST7102）宣传图" src="./images/product.png" width="640" /></p>

## 目录

- [产品简介](#产品简介)
- [规格参数](#规格参数)
- [示例工程](#示例工程)
- [仓库结构](#仓库结构)
- [相关资料](#相关资料)
- [购买链接](#购买链接)
- [技术支持](#技术支持)

---

## 产品简介

OSPTEK **4.3 寸 480×800 TFT** 是一款 **MIPI DSI** 接口彩色显示模组，显示驱动为 **ST7102**，触摸驱动为 **ST7123**。适合中小尺寸 HMI、手持终端与竖屏信息面板等场景。

规格标识（仓库名）：`4.3-tft-480x800-mipi-st7102`

当前模组版本：**YDP430BT009-V1**。电气与外形细节以 [`docs/YDP_430_BT_009_V1_a418b8470b.pdf`](./docs/YDP_430_BT_009_V1_a418b8470b.pdf) 为准。

## 规格参数

| 项目 | 规格 |
| ---- | ---- |
| 尺寸 | 4.3 英寸 |
| 类型 | TFT（彩色） |
| 分辨率 | 480×800 |
| 接口 | MIPI DSI |
| 驱动 IC | ST7102 |
| 触摸驱动 | ST7123 |

> 完整外形尺寸、FPC 定义、供电与时序以产品规格书 / 驱动手册为准。

## 示例工程

| 说明 | 路径 |
| ---- | ---- |
| ESP32-P4 · ST7102 MIPI + esp-lvgl-port / LVGL9 | [`examples/esp32p4-idf5_st7102-mipi_esp-lvgl-port_lvgl9/`](./examples/esp32p4-idf5_st7102-mipi_esp-lvgl-port_lvgl9/) |
| ESP32-P4 · 防撕裂 LVGL 演示 | [`examples/with-te/p4-idf_st7102-mipi_lvgl-common-demo/`](./examples/with-te/p4-idf_st7102-mipi_lvgl-common-demo/) |
| ESP32-P4 · ST7102 MIPI + SC2336 摄像头预览 | [`examples/camera/esp32p4-idf5_st7102-mipi-dsi_sc2336-mipi-csi_video-lcd-display/`](./examples/camera/esp32p4-idf5_st7102-mipi-dsi_sc2336-mipi-csi_video-lcd-display/) |
| Linux · RK3566 设备树 + ST7123 触摸参考 | [`examples/linux/`](./examples/linux/) |
| Raspberry Pi 5 · ST7102 480×800 面板驱动 / DT overlay（仅显示） | [`examples/rpi5-panel-st7102-480x800/`](./examples/rpi5-panel-st7102-480x800/) |
| Raspberry Pi 5 · ST7102 显示 + ST7123 触摸 / DT overlay | [`examples/rpi5-panel-st7102-st7123-480x800/`](./examples/rpi5-panel-st7102-st7123-480x800/) |
| Raspberry Pi 5 · ST7102 + ST7123 · LVGL（DRM + EVDEV） | [`examples/rpi5-lvgl-st7102-st7123-480x800/`](./examples/rpi5-lvgl-st7102-st7123-480x800/) |

## 仓库结构

```text
4.3-tft-480x800-mipi-st7102/                                # 仓库根（导航见 ../../README.md）
└── versions/
    └── YDP430BT009-V1/                                # 本料号完整资料
        ├── README.md
        ├── README_EN.md
        ├── images/
        ├── docs/
        └── examples/
```

## 相关资料

### 本产品资料

| 资料 | 链接 |
| ---- | ---- |
| 产品规格书（YDP430BT009-V1） | [`docs/YDP_430_BT_009_V1_a418b8470b.pdf`](./docs/YDP_430_BT_009_V1_a418b8470b.pdf) |
| 外形图（YDP430BT009-V1） | [`docs/YDP430BT009-V1_外形图.pdf`](./docs/YDP430BT009-V1_%E5%A4%96%E5%BD%A2%E5%9B%BE.pdf) |
| 3D 图纸（YDP430BT009-V1） | [`docs/YDP430BT009-V1.dwg`](./docs/YDP430BT009-V1.dwg) |
| 驱动 IC 数据手册（ST7102） | [`docs/ST7102_Datasheet_V0.22.pdf`](./docs/ST7102_Datasheet_V0.22.pdf) |
| 初始化序列（C） | [`docs/GX09C_ST7102+BOE4.3_2LANE_90HZ.c`](./docs/GX09C_ST7102+BOE4.3_2LANE_90HZ.c) |
| 时序配置参考图（90 Hz） | [`docs/RGB_Output_Timing_90Hz.jpg`](./docs/RGB_Output_Timing_90Hz.jpg) |
| 4.3 寸 LCD 转接板原理图 | [`docs/4.3寸LCD转接板V1.0.pdf`](./docs/4.3%E5%AF%B8LCD%E8%BD%AC%E6%8E%A5%E6%9D%BFV1.0.pdf) |

### 示例工程

- [ESP32-P4 ST7102 MIPI + LVGL9](./examples/esp32p4-idf5_st7102-mipi_esp-lvgl-port_lvgl9/)
- [ESP32-P4 防撕裂 LVGL 演示](./examples/with-te/p4-idf_st7102-mipi_lvgl-common-demo/)
- [ESP32-P4 ST7102 MIPI + SC2336 摄像头预览](./examples/camera/esp32p4-idf5_st7102-mipi-dsi_sc2336-mipi-csi_video-lcd-display/)
- [Linux RK3566 + ST7123 参考](./examples/linux/)
- [Raspberry Pi 5 ST7102 面板（仅显示）](./examples/rpi5-panel-st7102-480x800/)
- [Raspberry Pi 5 ST7102 显示 + ST7123 触摸](./examples/rpi5-panel-st7102-st7123-480x800/)
- [Raspberry Pi 5 ST7102 + ST7123 · LVGL](./examples/rpi5-lvgl-st7102-st7123-480x800/)

## 购买链接

<p align="center">
  <a href="https://shop110742373.taobao.com/"><img alt="淘宝官方店铺" src="https://img.shields.io/badge/淘宝-官方店铺-FF6A00?style=for-the-badge" /></a>
  &nbsp;&nbsp;
  <a href="https://www.aliexpress.com/store/1105701619"><img alt="速卖通官方店铺" src="https://img.shields.io/badge/速卖通-官方店铺-FF6A00?style=for-the-badge" /></a>
</p>

**国内（淘宝）**

- 店铺：[鱼鹰光电工厂店](https://shop110742373.taobao.com/)

**海外（AliExpress）**

- 店铺：[OSPTEK Official Store](https://www.aliexpress.com/store/1105701619)

## 技术支持

- 技术支持 / 产品咨询：<luyu@osptek.com>
- QQ 技术交流群：**985881096**
- 公司官网：<https://osptek.com/>
- 有任何问题，都可以在本仓库 Issues 中提问

---

<p align="center"><sub>© 2026 OSPTEK 鱼鹰光电 · 本仓库资料采用 CC BY 4.0 许可</sub></p>
