---
permalink: /
title: "Outdoor Urban Microclimate Sensing Device"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# 室外城市微氣候智能感知裝置
# Outdoor Urban Microclimate Sensing Device

## 項目簡介 / Project Overview

本項目開發了一套面向城市街區尺度的室外城市微氣候智能感知裝置，用於連續監測溫度、濕度、風速、風向、大氣壓強、太陽輻射和 GPS 位置信息等關鍵環境參數。裝置結合邊端控制、4G 通信、MQTT 數據傳輸與太陽能供電設計，支援長期戶外部署與雲端平台接入。

This project develops an outdoor intelligent sensing device for block-scale urban microclimate monitoring. It continuously measures key environmental parameters, including temperature, humidity, wind speed, wind direction, atmospheric pressure, solar radiation, and GPS location. The device integrates edge-side control, 4G communication, MQTT data transmission, and solar-powered operation, supporting long-term outdoor deployment and cloud-platform integration.

## 功能介紹 / Key Features

- 多要素微氣候監測：溫度、濕度、風速、風向、大氣壓強、太陽輻射與 GPS 定位
- 4G LTE + MQTT 無線數據傳輸
- 邊端數據處理、設備狀態監測與數據上傳調度
- 斷網緩存與自動補傳，提升長期監測數據完整性
- 太陽能供電與低功耗戶外運行
- 可接入智慧城市治理平台，用於熱風險識別、建築能耗分析和電網負荷研究

- Multi-parameter microclimate monitoring: temperature, humidity, wind speed, wind direction, atmospheric pressure, solar radiation, and GPS positioning
- 4G LTE and MQTT-based wireless data transmission
- Edge-side data processing, device-status monitoring, and data upload scheduling
- Offline caching and automatic retransmission to improve long-term data completeness
- Solar-powered and low-power outdoor operation
- Integration with smart city governance platforms for heat-risk identification, building-energy analysis, and power-load research

## 結構介紹 / System Structure

本裝置採用「感知—控制—通信—供電—平台」的一體化結構，主要由多功能氣象傳感器、太陽輻射傳感器、GPS 模組、ESP32 控制單元、4G 通信模組、MPPT 電源管理模組、電壓轉換模組和戶外安裝結構組成。其設計目標是實現從現場環境感知、邊端處理、無線傳輸到雲端分析的完整數據鏈路。

The device adopts an integrated sensing–control–communication–power–platform structure. It mainly consists of multi-functional meteorological sensors, a solar radiation sensor, a GPS module, an ESP32 control unit, a 4G communication module, an MPPT power-management module, a voltage-conversion module, and an outdoor mounting structure. The design aims to build a complete data pipeline from on-site environmental sensing and edge-side processing to wireless transmission and cloud-based analysis.

### 主要組成 / Main Components

| 模組 / Module | 說明 / Description |
|---|---|
| 感知模組 / Sensing Module | 採集溫度、濕度、風速、風向、大氣壓強、太陽輻射與位置數據。 Collects temperature, humidity, wind speed, wind direction, atmospheric pressure, solar radiation, and location data. |
| 控制模組 / Control Module | 以 ESP32 為核心，負責數據讀取、格式轉換、狀態判斷與上傳調度。 Uses ESP32 for data reading, format conversion, status detection, and upload scheduling. |
| 通信模組 / Communication Module | 通過 4G LTE 和 MQTT 協議將數據傳輸至雲端平台。 Transmits data to the cloud platform through 4G LTE and MQTT. |
| 供電模組 / Power Module | 結合太陽能供電、MPPT 控制和電壓轉換，支援長期戶外運行。 Integrates solar power, MPPT control, and voltage conversion for long-term outdoor operation. |
| 平台接口 / Platform Interface | 接入智慧城市治理平台，支援可視化、告警和跨領域數據分析。 Connects to the smart city governance platform for visualization, alerts, and cross-domain data analysis. |

## 應用場景 / Application Scenarios

本裝置可部署於建築密集區、校園、城市綠地、水體周邊、開闊廣場和道路空間，構建分佈式城市微氣候監測網絡，為「城市微氣候—電力—建築」交叉研究提供高時空分辨率數據支撐。

The device can be deployed in high-density building areas, campuses, urban green spaces, waterfront areas, open plazas, and street spaces. Through distributed deployment, it supports the construction of an urban microclimate monitoring network and provides high-resolution data for interdisciplinary research on urban microclimate, power systems, and buildings.
