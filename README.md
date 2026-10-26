# 📦 PapihaOS Project

<p align="center">
  <img src="https://githubusercontent.com" width="300" alt="PapihaOS Logo"><br>
  <b>Ultra-lightweight, high-performance custom Android firmware line for legacy and low-end devices.</b>
</p>

---

## 🚀 Философия проекта
**PapihaOS** — это авторская линейка облегчённых модификаций, созданная для тотального разгона старого кремния. Главная цель проекта — бескомпромиссная борьба с фоновыми задержками, шпионскими трекерами и тяжёлым заводским софтом ради освобождения каждого мегабайта оперативной памяти (ОЗУ).

### 🛠️ Ключевые особенности и оптимизация:
* **Тотальная дегуглизация (No GMS):** Полное удаление прожорливых Сервисов Google Play (`GmsCore`) и Google Фреймворка. Свободно до 40-50% больше ОЗУ из коробки.
* **Полное импортозамещение интерфейса:** Интеграция ультра-лёгких лаунчеров (Launcher3 AOSP) и встроенного независимого автономного маркета **OddMarket** для установки приложений без ввода аккаунтов.
* **Глубокие твики build.prop (ART VM Speed Mod):** Принудительное аппаратное ускорение графики (SurfaceFlinger) силами GPU, разгон отзывчивости тачскрина и оптимизация скроллинга.

---

## 📊 Текущий арсенал и статус сборок (Device List)

| Device | Status | Version | Download Link / Notes |
| :--- | :--- | :--- | :--- |
| **Fly IQ431** | 🟡 PLANNED | — | SW24_20150301 |
| **Alcatel POP C5 5036D** | 🟡 PLANNED | — | 01008_FT_Light |
| **MTC SMART START** | 🟡 PLANNED | — | MTS_Stock_FT_1.0.3 |
| **Nokia X** | 🟡 PLANNED | — | CyanogenMOD 10 RUS for Nokia X |
| **Samsung Galaxy Y Duos GT-S6102** | 🟡 PLANNED | — | DarkRom |
| **ZTE Blade AF3/A5** | 🟢 RELEASED | 1.0 | [Download]() (Port from Ark Benefit S451 AOSP) |
| **ZTE Blade A3** | 🟡 PLANNED | — | AOSP v1.0.4 |
| **ZTE Blade A5 PRO** | 🟡 PLANNED | — | FULL Stock Unlock v1.0.3 |
| **Micromax D303** | 🟡 PLANNED | — | SW_V11_HW_V1.0_22052015 |
| **Micromax D200** | 🟡 PLANNED | — | Russia_D200_SW_V0.0.9_HW_V1.0_090515 |
| **Lenovo A1000** | 🟢 RELEASED | 1.0.2 (FIX) | [Download]() (AOSP 5.0, 4PDA Released) |
| **Micromax Q346** | 🟡 PLANNED | — | SW_V009_HW_V2.0_20160114 |
| **Samsung Galaxy Mega 5.8 I9152** | 🔴 CANCELLED | — | Broadcom Capri CPU boot-lock. Defective eMMC partition sizing. |
| **ARK Benefit M1** | 🔴 CANCELLED | — | Can't find working factory firmware for this phone. |
| **Fly IQ239** | 🟡 PLANNED | — | sw19, sw20, sw22 |
| **Alcatel One Touch S'POP 4030D** | 🟡 PLANNED | — | 4030D_140814 |
| **Eltex NV-501 (PapihaOS Console Mod)** | 🔴 CANCELLED | — | Locked operator bootloader. Completely bypassed over the air via ADB. |

---

## 🛠️ Критический шаг после установки (Для сборок без SetupWizard)
При первом запуске Android может временно заблокировать шторку уведомлений и кнопку "Домой". Для исправления выполните эти команды на ПК через ADB-консоль:

```bash
adb shell settings put global device_provisioned 1
adb shell settings put secure user_setup_complete 1
```
После перезагрузки интерфейс и кнопка Домой будут полностью активны!

---
*Created by papiha (PapihaOS Team). Built for speed.*
