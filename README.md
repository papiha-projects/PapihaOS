# 📦 PapihaOS Project

<p align="center">
  <img src="PapihaOS%20Logo.jpg" width="300" alt="PapihaOS Logo"><br>
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

| Device | Status | Download Link | Version | Firmware basis / Notes |
| :--- | :--- | :--- | :--- | :--- |
| **Fly IQ431** | 🟠 PAUSED | — | — | Firmware paused for this reason: My phones don't have batteries. Once I buy one, I'll continue developing the firmware. |
| **Alcatel POP C5 5036D** | 🟡 PLANNED | — | — | 01008_FT_Light |
| **MTC SMART START** | 🟡 PLANNED | — | — | MTS_Stock_FT_1.0.3 |
| **Nokia X** | 🟡 PLANNED | — | — | CyanogenMOD 10 RUS for Nokia X |
| **Samsung Galaxy Y Duos GT-S6102** | 🟠 PAUSED | — | — | Firmware paused for this reason: The matrix on my phone died, it lights up white. Firmware development will continue after the matrix is replaced. |
| **ZTE Blade AF3/A5** | 🟢 RELEASED | [Download](https://github.com/papiha-projects/PapihaOS/releases#release-1.0-zte-af3) | 1.0 | Port from Ark Benefit S451 (AOSP) |
| **ZTE Blade A3** | 🟡 PLANNED | — | — | ZTE_CN_QB18D_P172R12V1.0.0B09/AOSP |
| **ZTE Blade A5 PRO** | 🔴 CANCELLED | — | — | Firmware canceled for this reason: The eMMC memory or processor on my phone is dead. |
| **Micromax D303** | 🟡 PLANNED | — | — | SW_V11_HW_V1.0_22052015 |
| **Micromax D200** | 🟠 PAUSED | — | — | Firmware paused for this reason: The charging port on my phone died. Firmware development has been temporarily paused and will resume after the port is replaced. |
| **Lenovo A1000** | 🟢 RELEASED | [Download](https://github.com/papiha-projects/PapihaOS/releases#release-v1.0.2-lenovo-a1000) | 1.0.2 (FIX) | AOSP 5.0 |
| **Micromax Q346** | 🟡 PLANNED | — | — | SW_V009_HW_V2.0_20160114 |
| **Samsung Galaxy Mega 5.8 I9152** | 🔴 CANCELLED | — | — | Firmware canceled for this reason: Broadcom Capri CPU boot-lock. Defective eMMC factory partition sizing and capricious bootloader structure. |
| **ARK Benefit M1** | 🔴 CANCELLED | — | — | Firmware canceled for this reason: I can't found firmware for this phone. |
| **Fly IQ239** | 🟡 PLANNED | — | — | sw19, sw20, sw22 |
| **Alcatel One Touch S'POP 4030D** | 🟡 PLANNED | — | — | 4030D_140814 |
| **Eltex NV-501 (PapihaOS Console Mod)** | 🔴 CANCELLED | — | — | Firmware canceled for this reason: Locked operator bootloader with security signatures blocks any local update files. Completely bypassed over the air via ADB console. |

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
