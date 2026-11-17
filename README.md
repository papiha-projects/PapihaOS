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

## 📱 Текущий арсенал и статус сборок (Device List)

| Device | Status | Download Link | Version | Firmware basis / Notes |
| :--- | :--- | :--- | :--- | :--- |
| **Fly IQ431** | 🟠 `IN PROGRESS` | — | — | Active development and testing in progress. |
| **Alcatel POP C5 5036D** | 🟡 `PLANNED` | — | — | 01008_FT_Light |
| **MTC SMART START** | 🔴 `CANCELLED` | — | — | Firmware canceled for this reason: All batteries and emmc died on my all phones. |
| **Nokia X** | 🔴 `CANCELLED` | — | — | Firmware canceled for this reason: Emmc on my phone died |
| **Samsung Galaxy Y Duos GT-S6102** | 🔴 `CANCELLED` | — | — | Firmware canceled for this reason: My phone turned out to be flooded and there is no point in restoring and replacing the matrix. |
| **ZTE Blade AF3/A5** | 🟢 `RELEASED` | [Download](https://github.com/papiha-projects/PapihaOS/releases#release-release-1.0.1-zte-af3) | 1.0.1 | Port from Ark Benefit S451 (AOSP) |
| **ZTE Blade A3** | 🟡 `PLANNED` | — | — | ZTE_CN_QB18D_P172R12V1.0.0B09/AOSP |
| **ZTE Blade A5 PRO** | 🔴 `CANCELLED` | — | — | Firmware canceled for this reason: The eMMC memory or processor on my phone is dead. |
| **Micromax D303** | 🟡 `PLANNED` | — | — | SW_V11_HW_V1.0_22052015 |
| **Micromax D200** | 🟠 `PAUSED` | — | — | Firmware paused for this reason: The charging port on my phone died. Firmware development has been temporarily paused and will resume after the port is replaced. |
| **Lenovo A1000** | 🟢 `RELEASED` | [Download](https://github.com/papiha-projects/PapihaOS/releases#release-v1.0.2-lenovo-a1000) | 1.0.2 (FIX) | AOSP 5.0 |
| **Micromax Q346** | 🟡 `PLANNED` | — | — | SW_V009_HW_V2.0_20160114 |
| **Samsung Galaxy Mega 5.8 I9152** | 🔴 `CANCELLED` | — | — | Firmware canceled for this reason: Broadcom Capri CPU boot-lock. Defective eMMC factory partition sizing and capricious bootloader structure. |
| **ARK Benefit M1** | 🔴 `CANCELLED` | — | — | Firmware canceled for this reason: I can't found firmware for this phone. |
| **Fly IQ239** | 🟠 `PAUSED` | — | — | Firmware paused for this reason: The touchscreen and battery on my phone died. Firmware development will continue after the touchscreen and battery is replaced. |
| **Alcatel One Touch S'POP 4030D** | 🟡 `PLANNED` | — | — | 4030D_140814 |
| **Eltex NV-501 (PapihaOS Console Mod)** | 🔴 `CANCELLED` | — | — | Firmware canceled for this reason: Locked operator bootloader with security signatures blocks any local update files. Completely bypassed over the air via ADB console. |
| **Fly IQ449** | 🟡 `PLANNED` | — | — | — |
| **Fly IQ430** | 🟡 `PLANNED` | — | — | — |

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
