# Павел Наумов — системный инженер

**Rust · C++ · Linux.** Делаю нативные программы и довожу до работы то, что «не заводится»:
порт игры на Linux, USB-транспорт для старых iPad, root-обвязку для телевизора,
детерминированное ядро реального времени, торговый стек с аварийным стопом.
17 лет в ИТ-инфраструктуре; локальный ИИ на своём железе (Xeon E5-2699 v3 + RTX 3090).

## 🔧 Что посмотреть

| Проект | Что это | Стек |
|---|---|---|
| [**Torgarik**](https://github.com/Bezooom/Torgarik) | Исследовательский торговый стек: walk-forward бэктест, проверка на отложенных данных, kill-switch, который блокирует живую торговлю, если стратегия не прошла проверку. Честный итог: «вживую не запускать». | Rust |
| [**yandex-messenger-native**](https://github.com/Bezooom/yandex-messenger-native) | Неофициальный нативный клиент Яндекс Мессенджера для Linux, релизы в `.deb` | Rust, GTK4, Libadwaita, GStreamer, SQLite |
| [**CnCGeneralsZH-Linux**](https://github.com/Bezooom/CnCGeneralsZH-Linux) | C&C Generals: Zero Hour нативно на Linux на основе [Reforged](https://github.com/olcayseygan/CnCGeneralsZH-Reforged): сборка, замеры X11 vs Wayland, заметки по рендеру | C++, Vulkan, SDL3 |
| [**takt-rt**](https://github.com/Bezooom/takt-rt) | Планировщик реального времени и парсер бинарного протокола без выделения памяти в горячем пути | C++20, lock-free, sanitizers в CI |
| [**Shnurok**](https://github.com/Bezooom/Shnurok) | Управление iPad с Linux + обход зависаний USB у A7/A8 на контроллерах ASMedia (передача через ep0, udev) | Python, libusb, udev |
| [**ochag-webos**](https://github.com/Bezooom/ochag-webos) | Свой домашний экран и демоны на root-нутом LG webOS 4.x + разбор 12 проблем прошивки | POSIX sh, init.d |

Ещё: [t1d-simulator](https://github.com/Bezooom/t1d-simulator) (численная модель транспорта кислорода),
[ignition-solver](https://github.com/Bezooom/ignition-solver) (жёсткий солвер на NumPy),
[Evocode](https://github.com/Bezooom/Evocode) (AI-IDE на базе VSCodium с локальными моделями).

## 🧭 Как я работаю

- **Сначала проверка, потом обещания.** У проектов есть тесты, CI или журнал замеров; цифры в README — из логов.
- **Нативно и просто.** Компилируемый код, systemd и shell вместо тяжёлых обёрток и лишних облаков.
- **Честные выводы.** Если идея не работает, проект так и пишет (см. Torgarik).
- **Данные остаются внутри.** Локальные модели и закрытый контур там, где облако нельзя.

## English

Systems engineer: **Rust, C++, Linux**. Native Linux apps (GTK4), game porting (Vulkan/SDL3),
USB & firmware workarounds, real-time C++, trading research tooling with hard safety gates,
on-prem AI on my own hardware. 17 years in IT infrastructure.

---

🌐 [naumovai.ru](https://naumovai.ru) · 𝕏 [@Bezooooom](https://x.com/Bezooooom) · ✉️ naumov122@gmail.com
