<p align="center">
  <img src="assets/banner.png" alt="ProxyShard" width="720">
</p>

<p align="center">
  <b>Clean proxies with UDP and p0f</b><br>
  for scraping, SEO, ads, anti-detect browsers, automation and e-commerce.
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
  <img alt="p0f" src="https://img.shields.io/badge/p0f-fingerprint%20switch-7C3AED?style=flat-square">
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

ProxyShard is a proxy infrastructure provider for teams, marketers, affiliates, developers and automation specialists who need stable, clean and flexible IPs for daily work.

### 🌐 Proxy types

| Type | Highlights |
| --- | --- |
| **Residential** | Real household IPs from 250+ locations, large rotating pool, geo targeting by country / region / city / ISP |
| **Premium residential** | Curated residential pool for the strictest targets |
| **Static ISP** | Static IPs from home internet providers · UDP + p0f · long-session stability |
| **Datacenter** | Dedicated 10G channels · low latency · UDP + p0f · one IP per customer |
| **Mobile** | Country and carrier targeting · link-based rotation · p0f support |

### ⚡ Protocols and features

- HTTP, SOCKS5 and **UDP** support (UDP via SOCKS5 on all products except US residential)
- **p0f** network fingerprint switching — see below
- Precise geo targeting by country, region, city and ISP
- Dedicated IPs on Datacenter and ISP — not shared
- Rotating and sticky sessions
- API access for proxy automation

### 🎭 Spotlight — p0f fingerprint spoofing

Every device transmits a TCP/IP-level fingerprint (MSS, TTL, TCP options, window size, TOS) that anti-fraud systems read. Most proxies run on Linux servers, so your "Windows" or "macOS" browser arrives with a Linux network signature — an instant red flag.

ProxyShard lets you pick the OS profile your proxy transmits:

**Windows 10 / 11** · **macOS** · **Linux** · **iOS** · **Android**

**Available on:** Datacenter · Static ISP · Mobile.

**Why it matters:** Google registration without p0f → phone verification almost every time. With p0f spoofing to Windows 10/11 → QR-code verification, the trusted-user path. Same applies to other anti-fraud systems that read network-layer signals.

[Read the full p0f guide →](https://docs.proxyshard.com/eng/our-products/p0f-spoofing)

### 🎯 Typical use cases

Web scraping · SERP and SEO monitoring · Ad verification · Affiliate marketing · Anti-detect browser setups · E-commerce and price tracking · QA and multi-region testing · AI automation · Social media workflows · Multi-accounting.

### 🧰 Free tools

| Tool | What it does | Open |
| --- | --- | --- |
| **Proxy Tester** | HTTP/SOCKS5 batch checker — connectivity, latency, status code, UDP detection for SOCKS5. Up to 100 proxies, 1 request per minute. ProxyShard account required. | [proxyshard.com/proxy-tester](https://proxyshard.com/proxy-tester) |
| **IP Checker** | Reveals the real IP behind a proxy, WebRTC leaks, browser anonymity score and 20+ browser fingerprint signals. No account required. | [proxyshard.com/ip-checker](https://proxyshard.com/ip-checker) |

**What the IP Checker analyzes** (severity: Critical → Low → Info):

- 🤖 **Automation detection** — WebDriver, Selenium and headless-browser artifacts
- 🖼️ **Hardware fingerprints** — Canvas, WebGL, Audio rendering
- 💻 **System properties** — CPU cores, RAM, fonts, screen resolution
- 🕒 **Behavioral markers** — timezone, language, DNT, ad blocker
- 📱 **Device emulation** — touch / pointer mismatches

### 🛠️ Official projects

| Repository | Purpose |
| --- | --- |
| [proxyshard-sdk-js](https://github.com/ProxyShard/proxyshard-sdk-js) | Official JavaScript / TypeScript SDK |
| [proxyshard-sdk-python](https://github.com/ProxyShard/proxyshard-sdk-python) | Official Python SDK |
| [p0f-profiles](https://github.com/ProxyShard/p0f-profiles) | p0f fingerprint presets |
| [blocklist](https://github.com/ProxyShard/blocklist) | Datacenter & ISP proxies blocklist |
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

Pick up a proxy from your ProxyShard dashboard, then use it like any HTTP or SOCKS5 proxy.

**curl (HTTP):**

```bash
curl -x http://USERNAME:PASSWORD@HOST:PORT https://api.ipify.org?format=json
```

**curl (SOCKS5):**

```bash
curl -x socks5://USERNAME:PASSWORD@HOST:PORT https://api.ipify.org?format=json
```

**Python (requests):**

```python
import requests

proxy = "http://USERNAME:PASSWORD@HOST:PORT"
resp = requests.get(
    "https://api.ipify.org?format=json",
    proxies={"http": proxy, "https": proxy},
    timeout=10,
)
print(resp.json())
```

**Node.js (undici):**

```js
import { fetch, ProxyAgent } from "undici";

const agent = new ProxyAgent("http://USERNAME:PASSWORD@HOST:PORT");
const res = await fetch("https://api.ipify.org?format=json", { dispatcher: agent });
console.log(await res.json());
```

For SDK-style access to the user API, see [proxyshard-sdk-js](https://github.com/ProxyShard/proxyshard-sdk-js) and [proxyshard-sdk-python](https://github.com/ProxyShard/proxyshard-sdk-python).

### ⚖️ Responsible use

ProxyShard is intended for legitimate automation, testing, monitoring and data access. We do not support spam, credential attacks, fraud, malware, or any activity that violates applicable laws or third-party terms.

- Business: **business@proxyshard.com**
- Abuse: **abuse@proxyshard.com**

---

<a id="-русский"></a>

## 🇷🇺 Русский

ProxyShard — прокси-инфраструктура для команд, маркетологов, арбитражников, разработчиков и специалистов по автоматизации, которым нужны стабильные, чистые и гибкие IP для повседневной работы.

### 🌐 Типы прокси

| Тип | Особенности |
| --- | --- |
| **Резидентные** | Реальные домашние IP из 250+ локаций, большой ротационный пул, гео по стране / региону / городу / провайдеру |
| **Премиум-резидентные** | Отобранный пул для самых строгих целей |
| **Статические ISP** | Статичные IP от домашних провайдеров · UDP + p0f · стабильность для долгих сессий |
| **Серверные** | Выделенные 10G каналы · низкий пинг · UDP + p0f · один IP на клиента |
| **Мобильные** | Таргетинг по стране и оператору · ротация по линку · поддержка p0f |

### ⚡ Протоколы и фичи

- HTTP, SOCKS5 и **UDP** (UDP через SOCKS5 на всех продуктах, кроме US residential)
- Подмена сетевого отпечатка **p0f** — см. ниже
- Точный гео-таргетинг по стране, региону, городу и провайдеру
- Выделенные IP на Datacenter и ISP — не делятся
- Ротационные и sticky-сессии
- API-доступ для автоматизации

### 🎭 Главное — подмена отпечатка p0f

У каждого устройства есть цифровой отпечаток на уровне TCP/IP (MSS, TTL, TCP options, window size, TOS), который читают антифрод-системы. Большинство прокси крутятся на Linux-серверах, поэтому «браузер Windows» приезжает с Linux-сигнатурой — мгновенный красный флаг.

ProxyShard позволяет выбрать, какой OS-профиль будет отдавать прокси:

**Windows 10 / 11** · **macOS** · **Linux** · **iOS** · **Android**

**Доступно на:** Datacenter · Static ISP · Mobile.

**Почему это важно:** регистрация в Google без p0f → почти всегда просит телефон. С подменой на Windows 10/11 → даёт QR-код, путь «доверенного пользователя». То же касается других антифрод-систем, читающих сетевые сигналы.

[Полный гайд по p0f →](https://docs.proxyshard.com/nashi-produkty/p0f-spoofing)

### 🎯 Типичные сценарии

Парсинг · мониторинг SERP и SEO · проверка рекламы · партнёрский маркетинг · антидетект-браузеры · мониторинг e-commerce и цен · QA и гео-тестирование · AI-автоматизация · соцсети · мультиаккаунтинг.

### 🧰 Бесплатные инструменты

| Инструмент | Что делает | Открыть |
| --- | --- | --- |
| **Proxy Tester** | Пакетная проверка HTTP/SOCKS5 — связь, latency, status code, проверка UDP для SOCKS5. До 100 прокси, 1 запрос в минуту. Нужен аккаунт ProxyShard. | [proxyshard.com/proxy-tester](https://proxyshard.com/proxy-tester) |
| **IP Checker** | Показывает реальный IP за прокси, утечки WebRTC, скоринг анонимности браузера и 20+ сигналов отпечатка. Аккаунт не нужен. | [proxyshard.com/ip-checker](https://proxyshard.com/ip-checker) |

**Что проверяет IP Checker** (уровни: Critical → Low → Info):

- 🤖 **Автоматизация** — WebDriver, Selenium и артефакты headless-браузеров
- 🖼️ **Аппаратные отпечатки** — Canvas, WebGL, Audio
- 💻 **Системные параметры** — ядра CPU, RAM, шрифты, разрешение экрана
- 🕒 **Поведенческие маркеры** — таймзона, язык, DNT, блокировщик рекламы
- 📱 **Эмуляция устройства** — несоответствия touch / pointer

### ⚖️ Ответственное использование

ProxyShard рассчитан на легитимную автоматизацию, тестирование, мониторинг и сбор данных. Мы не поддерживаем спам, атаки на учётки, мошенничество, malware и любые действия, нарушающие законы или правила третьих сторон.

- Business: **business@proxyshard.com**
- Abuse: **abuse@proxyshard.com**

---

<a id="-українська"></a>

## 🇺🇦 Українська

ProxyShard — проксі-інфраструктура для команд, маркетологів, арбітражників, розробників і фахівців з автоматизації, яким потрібні стабільні, чисті та гнучкі IP для щоденної роботи.

### 🌐 Типи проксі

| Тип | Особливості |
| --- | --- |
| **Резидентні** | Реальні домашні IP з 250+ локацій, великий ротаційний пул, гео за країною / регіоном / містом / провайдером |
| **Преміум-резидентні** | Відібраний пул для найсуворіших цілей |
| **Статичні ISP** | Статичні IP від домашніх провайдерів · UDP + p0f · стабільність для тривалих сесій |
| **Серверні** | Виділені 10G канали · низький пінг · UDP + p0f · один IP на клієнта |
| **Мобільні** | Таргетинг за країною й оператором · ротація за лінком · підтримка p0f |

### ⚡ Протоколи та можливості

- HTTP, SOCKS5 та **UDP** (UDP через SOCKS5 на всіх продуктах, крім US residential)
- Підміна мережевого відбитка **p0f** — див. нижче
- Точний гео-таргетинг за країною, регіоном, містом і провайдером
- Виділені IP на Datacenter і ISP — не діляться
- Ротаційні та sticky-сесії
- API-доступ для автоматизації

### 🎭 Головне — підміна відбитка p0f

У кожного пристрою є цифровий відбиток на рівні TCP/IP (MSS, TTL, TCP options, window size, TOS), який читають антифрод-системи. Більшість проксі працюють на Linux-серверах, тож «браузер Windows» приходить з Linux-сигнатурою — миттєвий червоний прапорець.

ProxyShard дозволяє обрати, який OS-профіль віддаватиме проксі:

**Windows 10 / 11** · **macOS** · **Linux** · **iOS** · **Android**

**Доступно на:** Datacenter · Static ISP · Mobile.

**Чому це важливо:** реєстрація в Google без p0f → майже завжди просить телефон. З підміною на Windows 10/11 → дає QR-код, шлях «довіреного користувача». Те саме стосується інших антифрод-систем, що читають мережеві сигнали.

[Повний гайд з p0f →](https://docs.proxyshard.com/nashi-produkty/p0f-spoofing)

### 🎯 Типові сценарії

Парсинг · моніторинг SERP та SEO · перевірка реклами · партнерський маркетинг · антидетект-браузери · моніторинг e-commerce та цін · QA та гео-тестування · AI-автоматизація · соцмережі · мультиакаунтинг.

### 🧰 Безкоштовні інструменти

| Інструмент | Що робить | Відкрити |
| --- | --- | --- |
| **Proxy Tester** | Пакетна перевірка HTTP/SOCKS5 — звʼязок, latency, status code, перевірка UDP для SOCKS5. До 100 проксі, 1 запит на хвилину. Потрібен акаунт ProxyShard. | [proxyshard.com/proxy-tester](https://proxyshard.com/proxy-tester) |
| **IP Checker** | Показує реальний IP за проксі, витоки WebRTC, скоринг анонімності браузера та 20+ сигналів відбитка. Акаунт не потрібен. | [proxyshard.com/ip-checker](https://proxyshard.com/ip-checker) |

**Що перевіряє IP Checker** (рівні: Critical → Low → Info):

- 🤖 **Автоматизація** — WebDriver, Selenium та артефакти headless-браузерів
- 🖼️ **Апаратні відбитки** — Canvas, WebGL, Audio
- 💻 **Системні параметри** — ядра CPU, RAM, шрифти, роздільна здатність екрана
- 🕒 **Поведінкові маркери** — таймзона, мова, DNT, блокувальник реклами
- 📱 **Емуляція пристрою** — невідповідності touch / pointer

### ⚖️ Відповідальне використання

ProxyShard призначений для легітимної автоматизації, тестування, моніторингу та збору даних. Ми не підтримуємо спам, атаки на акаунти, шахрайство, malware та будь-які дії, що порушують закони або правила третіх сторін.

- Business: **business@proxyshard.com**
- Abuse: **abuse@proxyshard.com**

---

<a id="-中文"></a>

## 🇨🇳 中文

ProxyShard 是面向团队、营销人员、流量套利者、开发者及自动化专家的代理基础设施服务,提供日常工作所需的稳定、干净、灵活的 IP。

### 🌐 代理类型

| 类型 | 特点 |
| --- | --- |
| **住宅代理** | 真实家庭 IP,覆盖 250+ 地区,大规模轮换池,可按国家 / 地区 / 城市 / 运营商定位 |
| **高级住宅代理** | 严格筛选的住宅池,适用于最苛刻的目标 |
| **静态 ISP** | 来自家庭运营商的静态 IP · UDP + p0f · 长会话稳定 |
| **数据中心** | 独享 10G 通道 · 低延迟 · UDP + p0f · 一人一 IP |
| **移动代理** | 按国家与运营商定位 · 通过链接轮换 · 支持 p0f |

### ⚡ 协议与特性

- 支持 HTTP、SOCKS5 与 **UDP**(UDP 通过 SOCKS5 在大部分产品上可用,美国住宅代理除外)
- **p0f** 网络指纹切换 — 详见下方
- 按国家、地区、城市和运营商进行精准地理定位
- Datacenter 与 ISP 代理为独享 IP,不与其他用户共享
- 轮换会话与粘性(sticky)会话
- 提供 API,用于代理自动化管理

### 🎭 重点功能 — p0f 网络指纹切换

每台设备都会传输 TCP/IP 层面的网络指纹(MSS、TTL、TCP options、window size、TOS),反欺诈系统会读取这些信号。绝大多数代理运行在 Linux 服务器上,因此"Windows"或"macOS"浏览器到达目标时携带的是 Linux 网络签名 — 这是非常明显的代理特征。

ProxyShard 允许你选择代理传输的操作系统指纹:

**Windows 10 / 11** · **macOS** · **Linux** · **iOS** · **Android**

**可用于:** 数据中心 · 静态 ISP · 移动代理。

**为什么重要:** 不使用 p0f 注册 Google 账号几乎每次都会要求手机验证;切换到 Windows 10/11 指纹后会显示二维码验证,即"可信用户"路径。其他读取网络层信号的反欺诈系统同样适用。

[阅读完整 p0f 指南 →](https://docs.proxyshard.com/nashi-produkty/p0f-spoofing)

### 🎯 典型使用场景

网页爬取 · SERP 与 SEO 监控 · 广告核验 · 联盟营销 · 反检测浏览器配置 · 电商与价格监控 · QA 与多地区测试 · AI 自动化 · 社交媒体工作流 · 多账号运营。

### 🧰 免费工具

| 工具 | 功能 | 打开 |
| --- | --- | --- |
| **Proxy Tester** | HTTP/SOCKS5 批量检测 — 连通性、延迟、状态码、SOCKS5 的 UDP 检测。单次最多 100 个代理,每分钟 1 次请求。需登录 ProxyShard 账号。 | [proxyshard.com/proxy-tester](https://proxyshard.com/proxy-tester) |
| **IP Checker** | 显示代理后的真实 IP、WebRTC 泄露、浏览器匿名性评分及 20+ 项浏览器指纹信号。无需账号。 | [proxyshard.com/ip-checker](https://proxyshard.com/ip-checker) |

**IP Checker 检测内容**(严重级别:Critical → Low → Info):

- 🤖 **自动化检测** — WebDriver、Selenium 及 headless 浏览器特征
- 🖼️ **硬件指纹** — Canvas、WebGL、Audio 渲染
- 💻 **系统参数** — CPU 核心数、内存、字体、屏幕分辨率
- 🕒 **行为标记** — 时区、语言、DNT、广告拦截器
- 📱 **设备模拟** — touch / pointer 不一致

### ⚖️ 合规使用

ProxyShard 仅供合法的自动化、测试、监控与数据访问用途。我们不支持垃圾邮件、账号攻击、欺诈、恶意软件以及任何违反适用法律或第三方条款的行为。

- 商务合作:**business@proxyshard.com**
- 滥用举报:**abuse@proxyshard.com**

---

<p align="center">
  <sub>© ProxyShard · <a href="https://proxyshard.com">proxyshard.com</a></sub>
</p>
