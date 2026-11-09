# Павел Наумов — системный инженер

<p align="center">
  <a href="https://naumovai.ru/"><img src="https://img.shields.io/badge/naumovai.ru-0A66C2?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website" /></a>
  <img src="https://img.shields.io/badge/Role-Systems_Engineer-10b981?style=for-the-badge" alt="Role" />
  <img src="https://img.shields.io/badge/Also-Engineering_Leadership-0ea5e9?style=for-the-badge" alt="Leadership" />
  <img src="https://img.shields.io/badge/Architecture-On--Premise_AI_%7C_Systems-8b5cf6?style=for-the-badge" alt="Focus" />
  <img src="https://img.shields.io/badge/Experience-17%2B_Years-f59e0b?style=for-the-badge" alt="Experience" />
  <img src="https://img.shields.io/badge/Security-Air--Gapped_%26_Zero--Trust-ef4444?style=for-the-badge" alt="Security" />
</p>

<p align="center">
  <img src="https://skillicons.dev/icons?i=rust,python,cpp,ts,linux,docker,sqlite,postgres,git,bash" alt="Core Technology Stack" />
</p>

---

## 🧭 Позиционирование и профиль

**Системный инженер: Rust · C++ · Linux.** Нативные программы, порт игры на Linux (Vulkan/SDL3), USB-транспорт для старых iPad, root-обвязка телевизора, детерминированное ядро реального времени, торговый стек с аварийным стопом.

Инженерный руководитель (VP of Engineering / Head of R&D / Principal Architect) с **17+ годами практики** в разработке наукоемкого ПО, построении критической ИТ-инфраструктуры и внедрении локальных систем искусственного интеллекта на промышленных предприятиях.

Специализируюсь на создании **суверенных On-Premise и Edge AI контуров**, где публичные облачные API неприменимы по соображениям государственной или коммерческой тайны (DLP, Air-Gapped периметры, защита от утечек исходного кода). Проектирую системы с жесткими ограничениями по ресурсам — от гарантированной работы на офисных CPU до распределенного инференса на GPU-кластерах NVIDIA.

---

## 🎯 Инженерный радар технологий (Tech Radar)

Радар отражает баланс между проверенными производственными стандартами и исследованиями с высоким бизнес-эффектом:

```mermaid
quadrantChart
    title Инженерный радар технологий и подходов
    x-axis "Исследование / Оценка" --> "Промышленный стандарт"
    y-axis "Вспомогательный контур" --> "Критическая инфраструктура"
    quadrant-1 "Core Production Stack"
    quadrant-2 "High-Impact R&D"
    quadrant-3 "Assess / Hold"
    quadrant-4 "Foundational Systems"
    "Rust (GTK4, Libadwaita, IPC)": [0.88, 0.84]
    "Python (FastAPI, PyTorch, asyncio)": [0.93, 0.90]
    "Local SLM & LLM (On-Prem / SGLang)": [0.76, 0.88]
    "DLP & Air-Gapped Enclaves": [0.82, 0.94]
    "SQLite FTS5 BM25 (Zero-GPU Search)": [0.89, 0.80]
    "GPU OCR (PaddleOCR v5, CUDA 12.8)": [0.74, 0.82]
    "Digital Twins & Multiphysics CFD": [0.65, 0.62]
    "Linux Daemons, systemd & Docker": [0.91, 0.76]
    "Public Cloud GenAI APIs": [0.22, 0.20]
```

---

## 🚀 Избранные публичные разработки (Open R&D)

<table width="100%">
  <tr>
    <td width="33%" valign="top">
      <h3>📈 <a href="https://github.com/Bezooom/Torgarik">Torgarik</a></h3>
      <p><b>Стек:</b> <code>Rust</code>, <code>Hyperliquid</code>, <code>MOEX ISS</code></p>
      <p>Исследовательский торговый стек с walk-forward бэктестом.</p>
      <ul>
        <li><b>Защита:</b> kill-switch блокирует живую торговлю, если стратегия не прошла проверку</li>
        <li><b>Качество:</b> 181 тест, CI, честный итог «вживую не запускать»</li>
      </ul>
    </td>
    <td width="33%" valign="top">
      <h3>🎮 <a href="https://github.com/Bezooom/CnCGeneralsZH-Linux">CnCGeneralsZH-Linux</a></h3>
      <p><b>Стек:</b> <code>C++</code>, <code>Vulkan</code>, <code>SDL3</code></p>
      <p>C&amp;C Generals: Zero Hour нативно на Linux на основе <a href="https://github.com/olcayseygan/CnCGeneralsZH-Reforged">Reforged</a>.</p>
      <ul>
        <li><b>Замеры:</b> X11 против Wayland, профилирование рендера</li>
        <li><b>Лицензия:</b> GPL v3 + условия EA, без игровых файлов</li>
      </ul>
    </td>
    <td width="33%" valign="top">
      <h3>⏱️ <a href="https://github.com/Bezooom/takt-rt">takt-rt</a></h3>
      <p><b>Стек:</b> <code>C++20</code>, <code>lock-free</code>, <code>SPSC</code></p>
      <p>Детерминированный планировщик реального времени и парсер бинарного протокола.</p>
      <ul>
        <li><b>Память:</b> без выделений в горячем пути</li>
        <li><b>CI:</b> сборка с -Werror, ASan/UBSan/TSan</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="33%" valign="top">
      <h3>🔌 <a href="https://github.com/Bezooom/Shnurok">Shnurok</a></h3>
      <p><b>Стек:</b> <code>Python</code>, <code>libusb</code>, <code>udev</code></p>
      <p>Управление iPad с Linux: файлы AFC, установка IPA, syslog.</p>
      <ul>
        <li><b>Низкий уровень:</b> обход зависаний USB у A7/A8 на ASMedia xHCI через ep0</li>
        <li><b>CI:</b> контрактные тесты протокола</li>
      </ul>
    </td>
    <td width="33%" valign="top">
      <h3>🔥 <a href="https://github.com/Bezooom/ochag-webos">ochag-webos</a></h3>
      <p><b>Стек:</b> <code>POSIX sh</code>, <code>init.d</code>, <code>webOS</code></p>
      <p>Свой домашний экран и демоны на root-нутом LG webOS 4.x.</p>
      <ul>
        <li><b>Демоны:</b> TorrServer на :8090, перехват кнопки Home</li>
        <li><b>Разбор:</b> 12 проблем прошивки, контрактные тесты в CI</li>
      </ul>
    </td>
    <td width="33%" valign="top">
      <h3>🦀 <a href="https://github.com/Bezooom/yandex-messenger-native">yandex-messenger-native</a></h3>
      <p><b>Стек:</b> <code>Rust</code>, <code>GTK4</code>, <code>Libadwaita</code>, <code>WebKitGTK</code></p>
      <p>Нативный десктопный клиент для Яндекс.Мессенджера под Linux в стандартах GNOME HIG.</p>
      <ul>
        <li><b>Footprint:</b> нативный GTK4 без Electron, релизы в <code>.deb</code></li>
        <li><b>Графика:</b> аппаратное ускорение рендеринга и полная поддержка Wayland</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="33%" valign="top">
      <h3>🧮 <a href="https://github.com/Bezooom/ignition-solver">ignition-solver</a></h3>
      <p><b>Стек:</b> <code>Python</code>, <code>NumPy</code>, <code>BDF2</code></p>
      <p>Солвер жёсткого тепломассопереноса на чистом NumPy.</p>
      <ul>
        <li><b>Метод:</b> BDF2 + BiCGSTAB с предобуславливателем</li>
        <li><b>Проверка:</b> контроль инварианта энергии</li>
      </ul>
    </td>
    <td width="33%" valign="top">
      <h3>🧬 <a href="https://github.com/Bezooom/Evocode">Evocode</a></h3>
      <p><b>Стек:</b> <code>VSCodium</code>, <code>Local LLM</code>, <code>DLP Engine</code></p>
      <p>Российская privacy-first AI-IDE на базе VSCodium со встроенной DLP-фильтрацией.</p>
      <ul>
        <li><b>Безопасность:</b> автоматический перехват секретов, токенов и PII в коде</li>
        <li><b>Автономия:</b> локальный инференс без передачи данных во внешние облака</li>
      </ul>
    </td>
    <td width="33%" valign="top">
      <h3>🫀 <a href="https://github.com/Bezooom/t1d-simulator">t1d-simulator</a></h3>
      <p><b>Стек:</b> <code>Python</code>, <code>CFD / FVM</code>, <code>SciPy</code></p>
      <p>Открытый калиброванный цифровой двойник для исследований диабета 1 типа.</p>
      <ul>
        <li><b>Модель:</b> кинетика диффузии кислорода и глюкозы в микрокапсулах</li>
        <li><b>Применение:</b> дизайн трансплантатов островковых клеток поджелудочной</li>
      </ul>
    </td>
  </tr>
</table>

---

## 🔒 Промышленный опыт и закрытые проекты (Enterprise & NDA)

Значительная часть архитектурной практики выполняется в рамках корпоративных соглашений о конфиденциальности:

<details open>
<summary><b>1. Интеллектуальный классификатор ТН ВЭД ЕАЭС и таможенный терминал</b></summary>
<br>

* **Задача:** Автоматизация предобработки международных товаросопроводительных документов (инвойсы, упаковочные листы, спецификации), детерминированное присвоение 10-значных кодов ТН ВЭД ЕАЭС и расчет таможенных платежей (пошлины ЕТТ, НДС, сборы по ПП РФ № 342).
* **Архитектура:**
  * Гибридный контур: GPU-ускоренный OCR (`PaddleOCR PP-OCRv5` на CUDA 12.8, **< 9 сек/стр**) с пространственной кластеризацией таблиц (`Spatial Bands`).
  * Детерминированное ядро классификации: редукция 12-значных иностранных GTIP к 6-значным субпозициям, FTS5 BM25 поиск с русской лемматизацией (`< 10 мс`).
  * **Trust Boundary (Граница доверия):** автоматическая блокировка автоприсвоения для оружия (группа 93), взрывчатки (группа 36), товаров двойного назначения (БПЛА, радиация, яды) и партий с пошлиной свыше 100 000 ₽.
  * **Human-in-the-Loop Review Queue:** очередь верификации эксперта с фиксацией нормативных оснований и неизменяемым журналом аудита.
* **Метрики качества:** замерялись на внутреннем тестовом наборе заказчика. Набор и цифры не публикуются (NDA), поэтому здесь их не привожу.
</details>

<details>
<summary><b>2. Автоматизация КТПП и MES-контуров в машиностроении</b></summary>
<br>

* **Контур:** Интеграция конструкторско-технологической подготовки производства (КТПП) с системами диспетчеризации цехов (MES) и складским учетом ERP.
* **Решения:** Проектирование нормативно-справочных баз изделий (BOM), построение расцеховки, детерминированные алгоритмы нормирования материалов и трудоемкости, синхронизация справочников в транзакционном режиме.
</details>

<details>
<summary><b>3. Локальные корпоративные RAG-системы и ассистенты инженеров</b></summary>
<br>

* **Контур:** Внедрение систем анализа внутренней конструкторской, технологической и нормативной документации (ГОСТ, ТУ, ОСТ).
* **Решения:** Air-gapped инсталляции на базе квантованных открытых моделей, гибридный поиск (BM25 + плотные векторные эмбеддинги), фильтрация галлюцинаций через жесткие цитатные барьеры и синтаксическую верификацию.
</details>

---

## 🏛 Инженерные принципы (Operating Philosophy)

1. **Детерминизм превыше генеративного хайпа:** в регулируемых отраслях (таможня, финансы, безопасность, медицина) алгоритм обязан давать проверяемый и юридически воспроизводимый результат. ИИ — это ассистент распознавания и поиска, но финальное решение фиксируется строгими правилами.
2. **Data Sovereignty by Design:** коммерческие документы, конструкторские чертежи и исходный код предприятия никогда не должны покидать внутренний контур сети.
3. **Lean Native Footprint:** отдаю предпочтение легковесному компилируемому коду (Rust, C++, оптимизированные расширения Python) вместо прожорливых браузерных контейнеров.
4. **Архитектура шести месяцев (Six-Month Maintainability):** отказ от избыточных фреймворков и хрупких абстракций в пользу простых, понятных и поддерживаемых решений.

---

## 🌍 English

Systems engineer: **Rust, C++, Linux**. Native Linux apps (GTK4), game porting (Vulkan/SDL3), USB & firmware workarounds, real-time C++, trading research tooling with hard safety gates, on-prem AI on my own hardware (Xeon E5-2699 v3 + RTX 3090). 17 years in IT infrastructure.

---

## 📬 Контакты и публикации

<p align="center">
  <a href="https://naumovai.ru/"><img src="https://img.shields.io/badge/Блог_и_кейсы-naumovai.ru-0A66C2?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Blog" /></a>
  <a href="mailto:naumov122@gmail.com"><img src="https://img.shields.io/badge/Email-naumov122%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://x.com/Bezooooom"><img src="https://img.shields.io/badge/X-@Bezooooom-000000?style=for-the-badge&logo=x&logoColor=white" alt="X" /></a>
  <a href="https://github.com/Bezooom"><img src="https://img.shields.io/badge/GitHub-Bezooom-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
</p>

---

<p align="center">
  <sub>© Павел Наумов &bull; Системный инжиниринг, автономия и прикладной ИИ без компромиссов в безопасности.</sub>
</p>
