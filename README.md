<p align="center">
  <img src="assets/banner.png" alt="ProxyShard" width="720">
</p>

<p align="center">
  <b>Proxy infrastructure for traffic, testing and automation</b><br>
  Residential, ISP, datacenter and mobile proxies for SEO, scraping, ad verification, anti-detect browsers and e-commerce workflows.
</p>

<p align="center">
  <a href="https://proxyshard.com"><img alt="Website" src="https://img.shields.io/badge/Website-proxyshard.com-7C3AED?style=for-the-badge&logo=googlechrome&logoColor=white"></a>
  <a href="https://docs.proxyshard.com"><img alt="Docs" src="https://img.shields.io/badge/Docs-docs.proxyshard.com-1F2937?style=for-the-badge&logo=gitbook&logoColor=white"></a>
  <a href="https://proxyshard.com/proxy-tester"><img alt="Proxy Tester" src="https://img.shields.io/badge/Tool-Proxy%20Tester-22C55E?style=for-the-badge&logo=speedtest&logoColor=white"></a>
  <a href="https://proxyshard.com/ip-checker"><img alt="IP Checker" src="https://img.shields.io/badge/Tool-IP%20Checker-0EA5E9?style=for-the-badge&logo=cloudflare&logoColor=white"></a>
  <a href="mailto:business@proxyshard.com"><img alt="Email" src="https://img.shields.io/badge/Business-business%40proxyshard.com-EF4444?style=for-the-badge&logo=maildotru&logoColor=white"></a>
</p>

<p align="center">
  <img alt="UDP" src="https://img.shields.io/badge/UDP-supported-22C55E?style=flat-square">
  <img alt="p0f" src="https://img.shields.io/badge/p0f-DC%20%7C%20ISP%20%7C%20Mobile-7C3AED?style=flat-square">
  <img alt="HTTP" src="https://img.shields.io/badge/HTTP-✓-1F2937?style=flat-square">
  <img alt="SOCKS5" src="https://img.shields.io/badge/SOCKS5-✓-1F2937?style=flat-square">
  <img alt="Locations" src="https://img.shields.io/badge/Locations-250%2B-0EA5E9?style=flat-square">
  <img alt="IP pool" src="https://img.shields.io/badge/IP%20pool-3M%2B-0EA5E9?style=flat-square">
</p>

<p align="center">
  <a href="#-english">🇺🇸 English</a> ·
  <a href="#-русский">🇷🇺 Русский</a> ·
  <a href="#-українська">🇺🇦 Українська</a> ·
  <a href="#-中文">🇨🇳 中文</a>
</p>

---

<a id="-english"></a>

## 🇺🇸 English

ProxyShard is a proxy infrastructure provider for marketers, affiliates, developers, SEO teams and automation specialists who need stable IPs, predictable sessions and flexible network settings for production workflows.

### 🌐 Proxy types

| Type | Highlights |
| --- | --- |
| **Residential** | Real home ISP IPs, large rotating pool, geo targeting by country, region and city |
| **Premium Residential** | Selected residential pool with ISP-level targeting, for stricter traffic environments and higher-trust workflows |
| **ISP** | Static IPv4 from genuine residential ISP allocations (not datacenter ranges relabeled as ISP), dedicated to a single customer (same as Datacenter), never shared between users |
| **Datacenter** | Fast dedicated IPv4 proxies, low latency, 10 Gbit/s channels, built for scale and automation |
| **Mobile** | 3G, 4G, 5G and LTE carrier IPs, country and operator targeting, sticky and rotating sessions |

### ⚡ Protocols and features

- **Protocols:** HTTP, SOCKS5, SOCKS5h and UDP
- **SOCKS5h:** hostname resolution happens at the proxy, the local resolver never sees the destination and DNS does not leak
- **UDP** via SOCKS5 UDP ASSOCIATE per [RFC 1928 §6](https://datatracker.ietf.org/doc/html/rfc1928#section-6) — see the UDP section below for product coverage
- **p0f network fingerprint switching** for Datacenter, ISP and Mobile proxies, supported on all Datacenter and ISP locations
- Geo targeting by country, region, city and mobile carrier where available; ISP-level targeting on Premium Residential
- Dedicated IPs for Datacenter and ISP proxies, never shared between customers
- Sticky and rotating sessions
- API access for orders, billing and balance, sub-user management, proxy generation, p0f add-ons and full workflow automation

### 🎭 p0f network fingerprint switching

Anti-fraud systems may evaluate more than the browser fingerprint. Network-level signals such as MSS, TTL, TCP options, window size and TOS can also be used to identify the operating system profile behind a connection.

ProxyShard allows users to switch the p0f network fingerprint profile for supported proxy types. This helps keep the proxy, browser profile and expected device environment technically consistent.

Available p0f profiles:

**Windows 10 / 11** · **macOS** · **Linux** · **iOS** · **Android**

**Available on:** Datacenter · ISP · Mobile.

**What this looks like in practice:** Google account registration without p0f typically requests phone verification. With p0f switched to Windows 10 / 11, the same flow more often shows QR-code verification, the trusted-user path. Other anti-fraud systems that read network-level signals behave similarly.

**Recommended combo:** Static ISP proxies + p0f + [Vision Browser](https://docs.proxyshard.com/eng/usage-instructions/antidetect-browsers/vision-browser). Residential-level IP trust, matching network fingerprint and browser-layer fingerprint coverage in one stack.

[Read the p0f guide →](https://docs.proxyshard.com/eng/our-products/p0f-spoofing)

### 💡 Why UDP matters

TCP-only proxies break WebRTC and QUIC traffic. Most Chromium-based antidetect browsers cannot route WebRTC through a TCP proxy, leaving the real IP exposed. Services like Discord already verify WebRTC presence via Hcaptcha-enterprise, so without UDP an "anonymous" session is detected on the first check.

ProxyShard supports **UDP over SOCKS5** implemented strictly per [RFC 1928 §6 (UDP ASSOCIATE)](https://datatracker.ietf.org/doc/html/rfc1928#section-6) — any RFC-compliant client (Vision Browser, modern proxy stacks) gets WebRTC and QUIC out of the box.

**Available on every product, except:**

- Standart and Unmetered Residential — US locations only
- Premium Residential — all locations

[Read more about UDP →](https://docs.proxyshard.com/eng/our-products/about-udp)

### 🎯 Common use cases

Web scraping · SERP and SEO monitoring · Ad verification · Affiliate marketing · Anti-detect browser profiles · E-commerce and price tracking · QA and multi-region testing · App testing · Market research · Workflow automation · Multi-accounting.

### 📋 Which proxy type to pick

| If you need... | Pick |
| --- | --- |
| Real household IPs for scraping, SEO, ad verification or geo-sensitive tasks | **Residential** |
| The cleanest residential pool for the strictest targets | **Premium Residential** |
| Long sessions, account workflows, anti-fraud-heavy targets | **Static ISP** |
| Maximum speed and volume for automation pipelines | **Datacenter** |
| Highest trust, app testing, carrier-bound use cases | **Mobile** |

### 🧰 Free tools

| Tool | What it does | Open |
| --- | --- | --- |
| **Proxy Tester** | Batch checker for HTTP and SOCKS5 proxies: connectivity, latency, status code and UDP detection for SOCKS5. Supports up to 100 proxies per check, with 1 request per minute. ProxyShard account required. | [proxyshard.com/proxy-tester](https://proxyshard.com/proxy-tester) |
| **IP Checker** | Shows the visible IP, geolocation, WebRTC status, browser anonymity score and 20+ browser fingerprint signals. No account required. | [proxyshard.com/ip-checker](https://proxyshard.com/ip-checker) |

**IP Checker analyzes:**

- 🤖 **Automation signals**: WebDriver, Selenium and headless-browser artifacts
- 🖼️ **Rendering fingerprints**: Canvas, WebGL and Audio
- 💻 **System properties**: CPU cores, RAM, fonts and screen resolution
- 🕒 **Environment markers**: timezone, language, DNT and ad blocker status
- 📱 **Device signals**: touch and pointer consistency

### 🛠️ Official projects

| Repository | Purpose |
| --- | --- |
| [proxyshard-sdk-js](https://github.com/ProxyShard/proxyshard-sdk-js) | Official JavaScript / TypeScript SDK |
| [proxyshard-sdk-python](https://github.com/ProxyShard/proxyshard-sdk-python) | Official Python SDK |
| [p0f-profiles](https://github.com/ProxyShard/p0f-profiles) | p0f fingerprint presets |
| [blocklist](https://github.com/ProxyShard/blocklist) | Datacenter and ISP proxy blocklist |
| [awesome-proxy](https://github.com/ProxyShard/awesome-proxy) | Curated proxy, automation and scraping resources |

### 📦 Supported proxy formats

```text
http://username:password@host:port
https://username:password@host:port
socks5://username:password@host:port
host:port:username:password
username:password@host:port
```

### 🚀 Quickstart

Take a proxy from the ProxyShard dashboard and use it as a standard HTTP or SOCKS5 proxy:

```bash
curl -x http://USERNAME:PASSWORD@HOST:PORT https://api.ipify.org?format=json
```

For ready-to-run Python recipes — generating residential proxy URLs with country / region / city targeting, listing Datacenter and ISP active proxies, health-checking through `ipapi.co`, resolving relay IPs — see the cookbooks:

| Cookbook | Repo |
| --- | --- |
| 🇺🇸 English | [proxyshard-api-examples](https://github.com/ProxyShard/proxyshard-api-examples) |
| 🇷🇺 Русский | [proxyshard-api-examples-ru](https://github.com/ProxyShard/proxyshard-api-examples-ru) |

### 📚 Setup guides

Step-by-step configuration in the docs:

- **Antidetect browsers:** [Vision Browser](https://docs.proxyshard.com/eng/usage-instructions/antidetect-browsers/vision-browser)
- **Browsers:** [Chrome + ZeroOmega](https://docs.proxyshard.com/eng/usage-instructions/browsers/chrome/zeroomega) · [Firefox + FoxyProxy](https://docs.proxyshard.com/eng/usage-instructions/browsers/mozilla-firefox/foxyproxy) · [Safari](https://docs.proxyshard.com/eng/usage-instructions/browsers/safari) · [Opera](https://docs.proxyshard.com/eng/usage-instructions/browsers/opera) · [Edge](https://docs.proxyshard.com/eng/usage-instructions/browsers/edge)
- **System-level:** [Windows](https://docs.proxyshard.com/eng/usage-instructions/windows) · [macOS](https://docs.proxyshard.com/eng/usage-instructions/macos) · [Linux](https://docs.proxyshard.com/eng/usage-instructions/linux) · [iOS / Android](https://docs.proxyshard.com/eng/usage-instructions/ios-android)
- **Telegram:** [setup guide](https://docs.proxyshard.com/eng/usage-instructions/telegram)

### ⚖️ Responsible use

ProxyShard is intended for legitimate automation, testing, monitoring and data access. We do not support spam, credential attacks, fraud, malware or any activity that violates applicable laws or third-party terms.

- Business: **business@proxyshard.com**
- Abuse: **abuse@proxyshard.com**

---

<a id="-русский"></a>

## 🇷🇺 Русский

ProxyShard — прокси-инфраструктура для маркетологов, affiliate-команд, разработчиков, SEO-специалистов и команд автоматизации, которым нужны стабильные IP, предсказуемые сессии и гибкие сетевые настройки для рабочих процессов.

### 🌐 Типы прокси

| Тип | Особенности |
| --- | --- |
| **Residential** | Реальные домашние IP от интернет-провайдеров, большой ротационный пул, геотаргетинг по стране, региону и городу |
| **Premium Residential** | Отобранный residential-пул с фильтрацией по ISP, для строгих traffic-сценариев и задач, где важен высокий уровень доверия к IP |
| **ISP** | Статические IPv4 из настоящих ISP-выделений (а не серверные подсети с переклеенным ярлыком ISP, как у многих на рынке), выдаются персонально одному клиенту (как и Datacenter), не делятся между клиентами |
| **Datacenter** | Быстрые выделенные IPv4-прокси, низкая задержка, 10 Гбит/с каналы, высокая скорость для автоматизации и больших объёмов |
| **Mobile** | IP из 3G, 4G, 5G и LTE-сетей, таргетинг по стране и оператору, sticky и rotating sessions |

### ⚡ Протоколы и возможности

- **Протоколы:** HTTP, SOCKS5, SOCKS5h и UDP
- **SOCKS5h:** DNS-имена разрешаются на стороне прокси, локальный резолвер не видит адрес назначения, DNS не утекает
- **UDP** через SOCKS5 UDP ASSOCIATE по [RFC 1928 §6](https://datatracker.ietf.org/doc/html/rfc1928#section-6) — продуктовое покрытие см. в секции UDP ниже
- **p0f network fingerprint switching** для Datacenter, ISP и Mobile proxies, на всех локациях Datacenter и ISP
- Геотаргетинг по стране, региону, городу и мобильному оператору, где доступно; фильтрация по ISP только на Premium Residential
- Выделенные IP для Datacenter и ISP proxies, не шарятся между клиентами
- Sticky и rotating sessions
- API для заказов, биллинга и баланса, управления суб-юзерами, генерации прокси, p0f-аддонов и полной автоматизации workflow

### 🎭 p0f network fingerprint switching

Антифрод-системы могут смотреть не только на браузерный fingerprint. Сетевые сигналы уровня TCP/IP, включая MSS, TTL, TCP options, window size и TOS, тоже могут использоваться для определения профиля операционной системы за подключением.

ProxyShard позволяет переключать p0f network fingerprint profile для поддерживаемых типов прокси. Это помогает согласовать прокси, браузерный профиль и ожидаемую среду устройства на сетевом уровне.

Доступные профили p0f:

**Windows 10 / 11** · **macOS** · **Linux** · **iOS** · **Android**

**Доступно для:** Datacenter · ISP · Mobile.

**Как это работает на практике:** регистрация Google-аккаунта без p0f почти всегда просит подтверждение по телефону. С переключением p0f на Windows 10 / 11 тот же флоу чаще показывает QR-код, путь «доверенного пользователя». Другие антифрод-системы, которые читают сетевые сигналы, ведут себя так же.

**Рекомендуемая связка:** Static ISP-прокси + p0f + [Vision Browser](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/antidetect-browsers/vision-browser). Резидентное доверие к IP, совпадение сетевого отпечатка и покрытие fingerprint на уровне браузера в одном стеке.

[Гайд по p0f →](https://docs.proxyshard.com/nashi-produkty/p0f-spoofing)

### 💡 Почему UDP важен

TCP-only прокси ломают WebRTC и QUIC. Большинство Chromium-based антидетект-браузеров не могут пропустить WebRTC через TCP-прокси, реальный IP утекает наружу. Сервисы вроде Discord уже проверяют наличие WebRTC через Hcaptcha-enterprise, так что без UDP «анонимная» сессия палится на первой же проверке.

ProxyShard поддерживает **UDP over SOCKS5**, реализованный строго по [RFC 1928 §6 (UDP ASSOCIATE)](https://datatracker.ietf.org/doc/html/rfc1928#section-6) — любой RFC-совместимый клиент (Vision Browser, современные proxy-стеки) получает WebRTC и QUIC «из коробки».

**Доступно на всех продуктах, кроме:**

- Standart и Unmetered Residential — только USA-локации
- Premium Residential — все локации

[Подробнее про UDP →](https://docs.proxyshard.com/nashi-produkty/about-udp)

### 🎯 Популярные сценарии

Web scraping · SERP и SEO-мониторинг · проверка рекламы · affiliate marketing · anti-detect browser profiles · e-commerce и мониторинг цен · QA и multi-region testing · тестирование приложений · market research · автоматизация рабочих процессов · мультиаккаунтинг.

### 🧰 Бесплатные инструменты

| Инструмент | Что делает | Открыть |
| --- | --- | --- |
| **Proxy Tester** | Пакетная проверка HTTP и SOCKS5 proxies: подключение, latency, status code и UDP detection для SOCKS5. До 100 прокси за одну проверку, 1 запрос в минуту. Требуется аккаунт ProxyShard. | [proxyshard.com/proxy-tester](https://proxyshard.com/proxy-tester) |
| **IP Checker** | Показывает видимый IP, геолокацию, WebRTC status, browser anonymity score и 20+ browser fingerprint signals. Аккаунт не требуется. | [proxyshard.com/ip-checker](https://proxyshard.com/ip-checker) |

**IP Checker анализирует:**

- 🤖 **Automation signals**: WebDriver, Selenium и артефакты headless-браузеров
- 🖼️ **Rendering fingerprints**: Canvas, WebGL и Audio
- 💻 **System properties**: ядра CPU, RAM, шрифты и разрешение экрана
- 🕒 **Environment markers**: timezone, language, DNT и статус ad blocker
- 📱 **Device signals**: согласованность touch и pointer

### 📚 Гайды по настройке

Пошаговая настройка в документации:

- **Антидетект-браузеры:** [Vision Browser](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/antidetect-browsers/vision-browser)
- **Браузеры:** [Chrome](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/browsers/chrome) · [Firefox](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/browsers/mozilla-firefox) · [Safari](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/browsers/safari) · [Opera](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/browsers/opera) · [Edge](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/browsers/edge)
- **Операционные системы:** [Windows](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/windows) · [macOS](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/macos) · [Linux](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/linux) · [iOS / Android](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/ios-android)
- **Telegram:** [инструкция](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/telegram)

### ⚖️ Ответственное использование

ProxyShard предназначен для легитимной автоматизации, тестирования, мониторинга и доступа к данным. Мы не поддерживаем спам, атаки на аккаунты, мошенничество, malware и любые действия, нарушающие законы или правила сторонних сервисов.

- Business: **business@proxyshard.com**
- Abuse: **abuse@proxyshard.com**

---

<a id="-українська"></a>

## 🇺🇦 Українська

ProxyShard — проксі-інфраструктура для маркетологів, affiliate-команд, розробників, SEO-фахівців і команд автоматизації, яким потрібні стабільні IP, передбачувані сесії та гнучкі мережеві налаштування для робочих процесів.

### 🌐 Типи проксі

| Тип | Особливості |
| --- | --- |
| **Residential** | Реальні домашні IP від інтернет-провайдерів, великий ротаційний пул, геотаргетинг за країною, регіоном і містом |
| **Premium Residential** | Відібраний residential-пул з фільтрацією за ISP, для строгих traffic-сценаріїв і задач, де важливий високий рівень довіри до IP |
| **ISP** | Статичні IPv4 зі справжніх ISP-виділень (а не серверні підмережі під виглядом ISP, як у багатьох на ринку), видаються персонально одному клієнту (як і Datacenter), не діляться між клієнтами |
| **Datacenter** | Швидкі виділені IPv4-проксі, низька затримка, канали 10 Гбіт/с, висока швидкість для автоматизації та великих обсягів |
| **Mobile** | IP із 3G, 4G, 5G та LTE-мереж, таргетинг за країною й оператором, sticky та rotating sessions |

### ⚡ Протоколи та можливості

- **Протоколи:** HTTP, SOCKS5, SOCKS5h та UDP
- **SOCKS5h:** DNS-імена розв'язуються на стороні проксі, локальний резолвер не бачить адресу призначення, DNS не витікає
- **UDP** через SOCKS5 UDP ASSOCIATE за [RFC 1928 §6](https://datatracker.ietf.org/doc/html/rfc1928#section-6) — продуктове покриття див. у секції UDP нижче
- **p0f network fingerprint switching** для Datacenter, ISP та Mobile proxies, на всіх локаціях Datacenter та ISP
- Геотаргетинг за країною, регіоном, містом та мобільним оператором, де доступно; фільтрація за ISP лише на Premium Residential
- Виділені IP для Datacenter та ISP proxies, не діляться між клієнтами
- Sticky та rotating sessions
- API для замовлень, білінгу й балансу, управління суб-юзерами, генерації проксі, p0f-аддонів і повної автоматизації workflow

### 🎭 p0f network fingerprint switching

Антифрод-системи можуть оцінювати не лише браузерний fingerprint. Мережеві сигнали рівня TCP/IP, зокрема MSS, TTL, TCP options, window size та TOS, також можуть використовуватися для визначення профілю операційної системи за підключенням.

ProxyShard дозволяє перемикати p0f network fingerprint profile для підтримуваних типів проксі. Це допомагає узгодити проксі, браузерний профіль і очікуване середовище пристрою на мережевому рівні.

Доступні профілі p0f:

**Windows 10 / 11** · **macOS** · **Linux** · **iOS** · **Android**

**Доступно для:** Datacenter · ISP · Mobile.

**Як це працює на практиці:** реєстрація Google-акаунту без p0f майже завжди просить підтвердження телефоном. З переключенням p0f на Windows 10 / 11 той самий флоу частіше показує QR-код, шлях «довіреного користувача». Інші антифрод-системи, що читають мережеві сигнали, поводяться так само.

**Рекомендована звʼязка:** Static ISP-проксі + p0f + [Vision Browser](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/antidetect-browsers/vision-browser). Резидентний рівень довіри до IP, збіг мережевого відбитка та покриття fingerprint на рівні браузера в одному стеку.

[Гайд з p0f →](https://docs.proxyshard.com/nashi-produkty/p0f-spoofing)

### 💡 Чому UDP важливий

TCP-only проксі ламають WebRTC та QUIC. Більшість Chromium-based антидетект-браузерів не можуть пропустити WebRTC через TCP-проксі, справжній IP витікає назовні. Сервіси на кшталт Discord уже перевіряють наявність WebRTC через Hcaptcha-enterprise, тож без UDP «анонімна» сесія палиться на першій же перевірці.

ProxyShard підтримує **UDP over SOCKS5**, реалізований строго за [RFC 1928 §6 (UDP ASSOCIATE)](https://datatracker.ietf.org/doc/html/rfc1928#section-6) — будь-який RFC-сумісний клієнт (Vision Browser, сучасні proxy-стеки) отримує WebRTC і QUIC «з коробки».

**Доступно на всіх продуктах, окрім:**

- Standart і Unmetered Residential — лише USA-локації
- Premium Residential — усі локації

[Детальніше про UDP →](https://docs.proxyshard.com/nashi-produkty/about-udp)

### 🎯 Популярні сценарії

Web scraping · SERP та SEO-моніторинг · перевірка реклами · affiliate marketing · anti-detect browser profiles · e-commerce та моніторинг цін · QA і multi-region testing · тестування застосунків · market research · автоматизація робочих процесів · мультиакаунтинг.

### 🧰 Безкоштовні інструменти

| Інструмент | Що робить | Відкрити |
| --- | --- | --- |
| **Proxy Tester** | Пакетна перевірка HTTP та SOCKS5 proxies: підключення, latency, status code та UDP detection для SOCKS5. До 100 проксі за одну перевірку, 1 запит на хвилину. Потрібен акаунт ProxyShard. | [proxyshard.com/proxy-tester](https://proxyshard.com/proxy-tester) |
| **IP Checker** | Показує видимий IP, геолокацію, WebRTC status, browser anonymity score та 20+ browser fingerprint signals. Акаунт не потрібен. | [proxyshard.com/ip-checker](https://proxyshard.com/ip-checker) |

**IP Checker аналізує:**

- 🤖 **Automation signals**: WebDriver, Selenium та артефакти headless-браузерів
- 🖼️ **Rendering fingerprints**: Canvas, WebGL та Audio
- 💻 **System properties**: ядра CPU, RAM, шрифти та роздільна здатність екрана
- 🕒 **Environment markers**: timezone, language, DNT та статус ad blocker
- 📱 **Device signals**: узгодженість touch і pointer

### 📚 Гайди з налаштування

Покрокове налаштування у документації:

- **Антидетект-браузери:** [Vision Browser](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/antidetect-browsers/vision-browser)
- **Браузери:** [Chrome](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/browsers/chrome) · [Firefox](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/browsers/mozilla-firefox) · [Safari](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/browsers/safari) · [Opera](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/browsers/opera) · [Edge](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/browsers/edge)
- **Операційні системи:** [Windows](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/windows) · [macOS](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/macos) · [Linux](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/linux) · [iOS / Android](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/ios-android)
- **Telegram:** [інструкція](https://docs.proxyshard.com/instrukciya-po-ispolzovaniyu/telegram)

### ⚖️ Відповідальне використання

ProxyShard призначений для легітимної автоматизації, тестування, моніторингу й доступу до даних. Ми не підтримуємо спам, атаки на акаунти, шахрайство, malware або будь-які дії, що порушують закони чи правила сторонніх сервісів.

- Business: **business@proxyshard.com**
- Abuse: **abuse@proxyshard.com**

---

<a id="-中文"></a>

## 🇨🇳 中文

ProxyShard 是面向营销团队、联盟团队、开发者、SEO 团队和自动化专家的代理基础设施服务，适用于需要稳定 IP、可控会话和灵活网络配置的生产级工作流。

### 🌐 代理类型

| 类型 | 亮点 |
| --- | --- |
| **Residential** | 来自真实家庭 ISP 的 IP，大型轮换池，支持按国家、地区和城市进行地理定位 |
| **Premium Residential** | 精选住宅 IP 池，支持按 ISP 定向，适用于更严格的流量环境和高信任度工作流 |
| **ISP** | 来自真实 ISP 分配的静态 IPv4 地址(并非伪装成 ISP 的数据中心 IP 段),与 Datacenter 一样独享给单个客户,不与其他用户共享 |
| **Datacenter** | 高速独享 IPv4 代理，低延迟，10 Gbit/s 通道，适合规模化任务和自动化 |
| **Mobile** | 来自 3G、4G、5G 和 LTE 运营商网络的 IP，支持国家和运营商定位、sticky 与 rotating sessions |

### ⚡ 协议与功能

- **协议:** HTTP、SOCKS5、SOCKS5h 与 UDP
- **SOCKS5h:** DNS 在代理端解析,本地解析器无法看到目标地址,DNS 不会泄漏
- **UDP** 通过 SOCKS5 UDP ASSOCIATE 实现,严格遵循 [RFC 1928 §6](https://datatracker.ietf.org/doc/html/rfc1928#section-6) — 产品覆盖范围见下方 UDP 章节
- **p0f network fingerprint switching** 适用于 Datacenter、ISP 和 Mobile proxies,在 Datacenter 与 ISP 的所有地区均支持
- 可按国家、地区、城市和可用的移动运营商进行地理定位;ISP 级定向仅在 Premium Residential 上提供
- Datacenter 与 ISP proxies 为独享 IP,不与其他客户共享
- 支持 sticky 与 rotating sessions
- 提供 API,涵盖订单、账单与余额、子用户管理、代理生成、p0f 增值服务,以及完整的 workflow 自动化

### 🎭 p0f network fingerprint switching

反欺诈系统可能不只检查浏览器指纹。TCP/IP 层的网络信号，例如 MSS、TTL、TCP options、window size 和 TOS，也可能用于判断连接背后的操作系统画像。

ProxyShard 允许用户为支持的代理类型切换 p0f network fingerprint profile。这有助于让代理、浏览器画像和预期设备环境在网络层保持一致。

可用的 p0f 配置:

**Windows 10 / 11** · **macOS** · **Linux** · **iOS** · **Android**

**适用于:** Datacenter · ISP · Mobile.

**实际效果:** 注册 Google 账号时若不使用 p0f,大多数情况下会被要求短信验证;切换到 Windows 10 / 11 的 p0f 后,同一流程更常显示二维码验证,即"可信用户"路径。其他读取网络层信号的反欺诈系统也呈现类似行为。

**推荐组合:** Static ISP 代理 + p0f + [Vision Browser](https://docs.proxyshard.com/eng/usage-instructions/antidetect-browsers/vision-browser)。住宅级 IP 信任、网络层指纹匹配、浏览器层指纹覆盖,三层叠加。

[阅读 p0f 指南 →](https://docs.proxyshard.com/eng/our-products/p0f-spoofing)

### 💡 为什么 UDP 重要

TCP-only 代理无法承载 WebRTC 与 QUIC 流量。大多数基于 Chromium 的反检测浏览器无法通过 TCP 代理转发 WebRTC,真实 IP 会直接泄露。Discord 等服务已经通过 Hcaptcha-enterprise 检测 WebRTC 是否启用,没有 UDP 的话,"匿名"会话在第一次检查时就会被识破。

ProxyShard 提供 **UDP over SOCKS5**,严格按照 [RFC 1928 §6 (UDP ASSOCIATE)](https://datatracker.ietf.org/doc/html/rfc1928#section-6) 实现 — 任何符合 RFC 的客户端(Vision Browser、现代 proxy 客户端)都能开箱即用地获得 WebRTC 与 QUIC。

**所有产品都支持,以下情况除外:**

- Standart 与 Unmetered Residential — 仅限 USA 地区
- Premium Residential — 所有地区

[详细了解 UDP →](https://docs.proxyshard.com/eng/our-products/about-udp)

### 🎯 常见使用场景

Web scraping · SERP 与 SEO monitoring · 广告验证 · affiliate marketing · anti-detect browser profiles · e-commerce 与价格监控 · QA 与多地区测试 · 应用测试 · market research · 工作流自动化 · 多账号运营。

### 🧰 免费工具

| 工具 | 功能 | 打开 |
| --- | --- | --- |
| **Proxy Tester** | HTTP 和 SOCKS5 proxies 批量检测：连接状态、latency、status code 以及 SOCKS5 的 UDP detection。每次最多 100 个代理，每分钟 1 次请求。需要 ProxyShard 账号。 | [proxyshard.com/proxy-tester](https://proxyshard.com/proxy-tester) |
| **IP Checker** | 显示可见 IP、地理位置、WebRTC status、browser anonymity score 和 20+ browser fingerprint signals。无需账号。 | [proxyshard.com/ip-checker](https://proxyshard.com/ip-checker) |

**IP Checker 分析：**

- 🤖 **Automation signals**：WebDriver、Selenium 和 headless browser artifacts
- 🖼️ **Rendering fingerprints**：Canvas、WebGL 和 Audio
- 💻 **System properties**：CPU 核心数、RAM、字体和屏幕分辨率
- 🕒 **Environment markers**：timezone、language、DNT 和 ad blocker 状态
- 📱 **Device signals**：touch 和 pointer 一致性

### 📚 设置指南

文档中的分步配置指南:

- **反检测浏览器:** [Vision Browser](https://docs.proxyshard.com/eng/usage-instructions/antidetect-browsers/vision-browser)
- **浏览器:** [Chrome + ZeroOmega](https://docs.proxyshard.com/eng/usage-instructions/browsers/chrome/zeroomega) · [Firefox + FoxyProxy](https://docs.proxyshard.com/eng/usage-instructions/browsers/mozilla-firefox/foxyproxy) · [Safari](https://docs.proxyshard.com/eng/usage-instructions/browsers/safari) · [Opera](https://docs.proxyshard.com/eng/usage-instructions/browsers/opera) · [Edge](https://docs.proxyshard.com/eng/usage-instructions/browsers/edge)
- **操作系统:** [Windows](https://docs.proxyshard.com/eng/usage-instructions/windows) · [macOS](https://docs.proxyshard.com/eng/usage-instructions/macos) · [Linux](https://docs.proxyshard.com/eng/usage-instructions/linux) · [iOS / Android](https://docs.proxyshard.com/eng/usage-instructions/ios-android)
- **Telegram:** [配置指南](https://docs.proxyshard.com/eng/usage-instructions/telegram)

### ⚖️ 合规使用

ProxyShard 仅供合法的自动化、测试、监控与数据访问用途。我们不支持垃圾邮件、账号攻击、欺诈、恶意软件或任何违反适用法律和第三方条款的行为。

- 商务合作:**business@proxyshard.com**
- 滥用举报:**abuse@proxyshard.com**

---

<p align="center">
  <sub>© ProxyShard · <a href="https://proxyshard.com">proxyshard.com</a></sub>
</p>
