# PapihaOS
Official source code for PapihaOS project. Ultra-lightweight and optimized custom AOSP firmware line for legacy Android devices.
# 📦 PapihaOS Project

<p align="center">
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

## 📱 Текущий арсенал сборок (2026)

*   **ZTE Blade AF3 / A5 [v1.0]** — Чистый стабильный AOSP-базис.
*   **Lenovo A1000 [v1.0.2]** — Облегчённый Lollipop релиз с монументальным фиксом шторки. Опубликован в каталоге прошивок на **4PDA**.
*   **Eltex NV-501 [Console Mod]** — Беспроводной хак провайдерских приставок через ADB.

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
