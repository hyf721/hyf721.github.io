---
title: "BLE RX Sensitivity 的規格要求"
date: 2025-06-18T14:30:00+08:00
draft: false

# post thumb
image: "images/post/post-3.jpgx"

# meta description
description: "BLE RX Sensitivity 規格描述的相關規定"

# taxonomies
categories:
  - "Wi-Fi 筆記分享"
tags:
  - "Photos"

# post type
type: "post"
---
Bluetooth SIG 規範中對 RX Sensitivity 的要求

在 Bluetooth SIG 的核心規範（Bluetooth Core Specification）中，對於RX Sensitivity（接收靈敏度）的要求，會依不同藍牙技術類型（Classic vs. BLE）而有所不同。以下是針對 Bluetooth Low Energy（BLE）的接收靈敏度要求(根據 Bluetooth Core Specification v5.3/v5.4)

BLE 接收靈敏度要求（RX Sensitivity Requirement）
基本要求（Minimum RX Sensitivity）
在以下條件下，BLE 接收器需能正常接收資料：

•	測試條件：

  封包類型：PRBS9 資料模式
  
  封包長度：37 bytes（含 payload）

  頻率偏移：±150 kHz（如適用）

  訊號格式：GFSK

  錯誤率標準：PER ≤ 30%

•	靈敏度門檻：

  -70 dBm 或更好（即 ≤ -70 dBm 都可接受）

換句話說，BLE 的 RX Sensitivity 至少要達到 -70 dBm（在無干擾情況下仍能維持 PER ≤ 30%）


先查詢
Spec:
BT core spec. 5.4
https://www.bluetooth.com/specifications/specs/core-specification-5-4/

Page. 2655

![image](images/post/BTCore.png)

測試 37 Bytes 可推算出 BER 0.1% 約為 PER 30% (Follow下方R&S, 測試手冊)
意思是要測試在<=30% PER EUT 能測到最低的Power, 標準是 -70 dBm, 一般BLE chip可以測到 -90 ~ -100 dBm區間

https://scdn.rohde-schwarz.com/ur/pws/dl_downloads/dl_application/application_notes/1ma282/1MA282_BT_IOT_4e.pdf
![image](images/post/RS.png)




