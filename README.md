# Awesome-Android-IOS-Emulators-And-Simulators

**Top Android IOS Emulators And Simulators (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Virtual Devices, Browser-Based Streaming, Device Farms & Self-Hosted Emulation*

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Android & iOS Emulators and Simulators**. These tools enable developers and QA teams to run mobile apps without physical devices—from fully managed cloud device farms with real-device parity to self-hosted emulators that give teams control over their testing infrastructure and data.



**Examples** include BrowserStack, Sauce Labs, LambdaTest, Genymotion Cloud, Appetize.io, Corellium, Android Studio AVD, Xcode Simulator, BlueStacks, and NoxPlayer (the category leaders in commercial and open-source space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted mobile emulation, browser streaming, and open device farms. **Critical note**: The open-source landscape is genuinely functional—**tapflow** is the most complete self-hosted BrowserStack/Appetize alternative, streaming iOS simulators and Android emulators to any browser from your own Macs , **GADS** provides a full device farm with Appium integration and WebRTC streaming , and **dockerify-android** offers a Dockerized Android emulator with web access via scrcpy . For classic iOS apps, **TouchHLE** and **LightTouch** provide high-level emulation without requiring Apple hardware. No open-source project matches Corellium's full iOS virtualization or BrowserStack's real-device parity, but for simulator/emulator-based testing, the options are production-capable.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

| Product | Description | Starting Pricing | Free Tier / Trial Limits | Best For / Key Trade-off |
| :--- | :--- | :--- | :--- | :--- |
| **BrowserStack** | Cloud device farm with real devices and emulators. | • **App Live (Manual):** Starts at **$39/mo** (billed annually) or **$49/mo** (monthly) for 1 user seat.<br>• **App Automate:** Starts at **$199/mo** (billed annually) or **$249/mo** (monthly) for 1 parallel test run. | • **No permanent free tier** for App Live/Automate.<br>• **App Live Free Trial:** 30 total minutes across real devices (~1 min per session).<br>• **App Automate Free Trial:** 100 automated testing minutes.<br>• Qualifying open-source projects receive free testing plans. | **Best for:** Teams wanting real-device parity and cross-platform mobile testing.<br>**Trade-off:** Costs scale quickly with parallel test execution. |
| **Sauce Labs** | Enterprise cloud testing platform with virtual and real mobile devices. | • **Live Testing (Manual):** Starts at **$39/mo** (billed annually) or **$49/mo** (monthly).<br>• **Virtual Device Cloud (Automated):** Starts at **$149/mo** (billed annually) or **$199/mo** (monthly).<br>• **Real Device Cloud:** Starts at **$199/mo** (billed annually) or **$249/mo** (monthly). | • **No permanent free tier**.<br>• **28-Day Free Trial:** 60 automated & live testing minutes, up to 3 parallel virtual machines.<br>• Free sponsorship tier for open-source projects. | **Best for:** Enterprises needing both virtual and physical devices with strict enterprise compliance.<br>**Trade-off:** Inflexible pricing packages for smaller teams. |
| **LambdaTest** | Cloud mobile and browser testing platform offering virtual emulators/simulators and real devices. | • **Live Testing (Virtual):** Starts at **$15/mo** (billed annually) or **$19/mo** (monthly).<br>• **Automation Testing:** Starts at **$79/mo** (billed annually) or **$99/mo** (monthly).<br>• **HyperExecute:** Starts at **$159/mo** (billed annually). | • **Free Forever Plan:** 60 lifetime minutes of live testing (capped at 10-minute sessions), 100 automation minutes, and 2,000 SmartUI visual testing screenshots per month. | **Best for:** Budget-conscious teams needing affordable access to cloud emulators and fast test execution.<br>**Trade-off:** Physical real-device access requires costlier add-ons. |
| **Genymotion Cloud** | Cloud-based Android emulation available via SaaS web streaming and PaaS marketplace images. | • **Genymotion SaaS (Pay-as-you-go):** **$0.05 per minute** per active virtual device (no base subscription fee).<br>• **Genymotion Cloud Marketplace (AWS/GCP/Azure):** Hourly PaaS software fees from **~$0.50/hour** + cloud compute costs. | • **Genymotion SaaS Trial:** 60 free minutes total, capped at 2 concurrent virtual devices.<br>• **GCP Marketplace Trial:** 5-day trial with $60 Genymotion software credit (infrastructure charges still apply). | **Best for:** Teams and CI pipelines requiring scalable, high-performance cloud Android emulation.<br>**Trade-off:** Android-only; iOS devices and simulators are not supported. |
| **Appetize.io** | Browser-based interactive streaming for iOS and Android applications. | • **Starter Plan:** **$59/mo** (billed monthly) or **$50/mo** (billed annually), includes 500 streaming minutes ($0.06/min overage).<br>• **Premium Plan:** Starts at **$199/mo** (billed monthly). | • **Free Forever Tier:** 30 minutes per month total, capped at 3 minutes per session, and up to 2 concurrent active device streams. | **Best for:** Embedding interactive app demos in documentation, customer support, or beta testing in web browsers.<br>**Trade-off:** Streaming and manual presentation focus; not a full automated testing matrix. |
| **Corellium** | Virtualized ARM-based mobile device modeling engine for iOS and Android security research. | • **Solo Explorer Tier:** Starts at **$3.00 per device-hour**.<br>• **Enterprise / Viper:** Annual licensing starting at **$9,995/year** (bundles ~1,250 device-hours/mo). | • **No permanent free tier**.<br>• **Free Trial:** Available by request on a case-by-case basis (requires manual vetting and compliance approval); Arm Virtual Hardware (AVH) offers a 30-day trial with 100 core-hours and 15 simultaneous cores. | **Best for:** Security researchers, reverse engineers, and pentesting teams requiring rooted, low-level iOS firmware virtualization.<br>**Trade-off:** High starting price point; requires specialized technical expertise. |
| **Android Studio AVD** | Official local Android emulator bundled with Google's Android Studio IDE. | • **100% Free** (Open-source SDK tools and system images bundled with Android Studio). | • **Free Forever:** Unlimited local usage without any time limits, caps, or fees. | **Best for:** Native Android developers wanting the official, fully featured Google APIs and system images.<br>**Trade-off:** Resource-heavy local CPU/RAM footprint; no iOS support. |
| **Xcode Simulator** | Official local iOS, iPadOS, watchOS, and tvOS simulator bundled with Apple Xcode. | • **100% Free** with an Apple ID and Xcode on macOS. | • **Free Forever:** Unlimited local simulation without any time limits or usage caps. | **Best for:** iOS developers requiring swift, high-fidelity app simulation and native debugging.<br>**Trade-off:** macOS exclusive; requires high local disk space (15GB+). |
| **BlueStacks** | Consumer-oriented Android application emulator designed for desktop gaming. | • **Free with ads**.<br>• **BlueStacks Prime (Ad-Free):** **$7.99/mo** (monthly subscription removing all UI ads and providing 800 nowBux + 5,000 AI credits). | • **Free Forever Tier:** Ad-supported free tier with unlimited play time and multi-instance support. | **Best for:** Consumers and gamers wanting to run Android mobile games on PC/Mac.<br>**Trade-off:** Heavy advertising on free tier; unsuitable for CI/CD or automated developer testing. |
| **NoxPlayer** | Consumer Android desktop emulator optimized for mobile gaming and multitasking. | • **Free with ads**.<br>• **NoxPlayer Premium (VIP):** Starts at **$3.69/mo**, **$9.99/quarter**, or **$31.99/year** (removes launcher banner and startup ads across up to 5 instances). | • **Free Forever Tier:** Ad-supported free tier with unlimited usage and multi-instance support. | **Best for:** Gamers and everyday users wanting a lightweight Android game emulator on desktop.<br>**Trade-off:** Free tier includes launcher ads and sponsored game recommendations; not intended for developer QA/automation. |



## Open-Source GitHub Projects



- **tapflow**

  **Self-hosted Appetize/BrowserStack alternative** (MIT) — **the most complete open-source browser-based simulator streaming platform** found in this research . **Features**: **Browser streaming**—iOS & Android at ~30 fps with H.264 (WebCodecs on HTTPS, WASM fallback on HTTP), JPEG fallback for older browsers; **Touch, swipe & pinch** forwarded in real time; **Clipboard sync**, device audio, and network control (offline testing); **App Center** for uploading `.app.zip`/`.apk` and tracking builds; **Session recordings** kept 72 hours; **Screenshot REST endpoint** for CI/AI agents; **Flow runner** for deterministic QA flows; **MCP Server** (`@tapflowio/mcp-server`) for Claude Code and LLM agents; **Mac resource monitoring** and team management (Admin/Developer/QA/Viewer roles) . **Requirements**: Relay (Node.js ≥20, any OS, ~512MB RAM); Agent (macOS with Xcode/Android Studio); Browser (any modern) . **Deploy**: `npm install -g tapflow`; `tapflow setup` on Mac; `tapflow start`; dashboard at `http://localhost:4000` . **Trade-off**: **Agents run on macOS only**—requires Macs with Xcode/Android Studio; not a device farm; does not integrate with Appium/WebDriverAgent (ships its own runner) . **Best for**: teams with existing Macs wanting to share simulators/emulators with the whole team via browser—especially those wanting data sovereignty and no cloud uploads .



- **GADS**

  **Simple device farm for remote control and Appium testing** (AGPL-3.0, with proprietary hub-ui) — **the most complete open-source device farm** for iOS/Android with Appium integration . **Features**: **Device control**—real-time video streaming (MJPEG/WebRTC), tap/swipe/text input, keyboard typing, app installation, screenshots, device reservation; **Authentication**—user login, admin management, multiple JWT providers, OAuth2 for Appium; **Workspace management**—user access control per workspace; **Provider setup**—UI-based device management, automated Appium server configuration per device, optional Selenium Grid 4 node registration; **Smart TV testing**—Samsung Tizen and LG WebOS (automation only) . **Platform support**: macOS (full Android/iOS), Linux (limited iOS, full Android), Windows (limited iOS, full Android) . **Deploy**: Self-hosted (provider + hub architecture) . **Trade-off**: **Proprietary hub-ui** is obfuscated—not fully open source; iOS support requires Xcode (Mac only) . **Best for**: teams wanting a self-hosted device farm with Appium integration and remote control—especially those with mixed Android/iOS devices .



- **dockerify-android**

  **Dockerized Android emulator with web access** (open source) — **the easiest way to run a headless Android emulator with browser access** . **Features**: **Web interface** via scrcpy-web—no additional software, full touchscreen/keyboard support; **ARM translation** via ndk_translation for ARM-only apps on x86_64; **Root and Magisk preinstalled**; **PICO GAPPS** for Google services; **ADB access** from host and networked devices; **scrcpy support** for desktop mirroring; **Docker integration** with `docker compose up -d` . **Requirements**: Docker, KVM support (check `egrep -c '(vmx|svm)' /proc/cpuinfo`) . **Deploy**: `git clone` repo; `docker compose up -d`; web interface at `http://localhost:8000` . **Trade-off**: **Android-only**—no iOS support; requires KVM for performance . **Best for**: developers wanting a reproducible, containerized Android emulator with web access—especially those already using Docker .



- **AppiumTestDistribution/appium-device-farm**

  **Appium 2.0 plugin for device management** (open source, 262 stars) — **the most starred open-source device farm plugin** for Appium . **Features**: **Device allocation**—manages and creates driver sessions on available devices; **Appium integration**—works within Appium 2.0 ecosystem; **TypeScript** implementation . **Deploy**: Appium plugin (`appium plugin install`). **Trade-off**: **Plugin, not a standalone farm**—requires Appium infrastructure; no built-in UI for remote control . **Best for**: teams already using Appium wanting automated device allocation .



- **TouchHLE**

  **High-level iPhone emulator for classic apps** (open source, Rust) — **the most practical open-source iOS emulator for legacy apps**, running on Windows, macOS, and Android . **Features**: **High-level emulation**—reimplements UIKit, OpenGL ES, and OpenAL natively; only ARM binary is emulated via dynarmic; **Compatibility database**—153 of 667 tested apps work perfectly, 101 playable with minor bugs; includes Super Monkey Ball, Doom, Sonic, Angry Birds, Cut the Rope . **Limitations**: **32-bit only**—designed for iPhone OS 2.x and 3.0 era; **cannot run on iOS itself** (requires JIT, blocked by Apple) . **Deploy**: GitHub releases for Windows/macOS/Android; requires your own `.ipa` files . **Trade-off**: **Classic apps only**—not for modern 64-bit apps; no networking or full hardware emulation . **Best for**: preserving and playing classic iPhone games from 2008–2011 without Apple hardware .



- **LightTouch / LightTouchMac**

  **QEMU-based iOS emulator for classic devices** (open source) — **the most capable open-source classic iOS emulation** . **Features**: **LightTouchMac** (macOS only)—emulates original iPhone, iPhone 3GS, iPhone 4 GSM, iPod touch 1–4, first iPad; firmware from iPhone OS 1.x to iOS 7.1.2; touchscreen, graphics, audio, Wi-Fi, simulated cellular, persistent storage, media importing; **LightTouch** (cross-platform)—Android, Linux, Windows, macOS; shared QEMU-iOS engine; automatic IPSW firmware preparation; ipa installation; Legacy Store access; networking via Internet Archive Wayback Machine . **Requirements**: LightTouchMac requires macOS 14.4+ (Apple silicon or Intel); LightTouch Android requires ARM64 + Android 10+; Linux x86-64 AppImage; Windows x86-64 ZIP; macOS Apple silicon + macOS 26 . **Deploy**: LightTouchMac (macOS app); LightTouch (cross-platform downloads) . **Trade-off**: **Experimental**—many device/firmware combinations untested; original iPhone/iPod touch 1G stop at white screen . **Best for**: users wanting to run classic iOS apps and games across platforms—especially those with existing `.ipa` files .



### Additional Strong Open-Source Options



- **NixDroid** — x86_64 AOSP emulator for Linux (Beta, GitHub). Uses QEMU virtualization for native performance; root via Magisk; installer script . **Note**: **Linux-only, Beta**—requires KVM; active testing phase . **Best for**: Linux users wanting a native-performance Android emulator.

- **WayDroid** — Container-based Android for Linux (GPL-3.0). Runs full Android in a container using Linux namespaces; not an emulator—shares host kernel . **Note**: **Android-only**; not for iOS testing; requires Linux . **Best for**: Linux users wanting Android apps with near-native performance .

- **OpenSTF (STF)** — Control and manage Android devices from browser (open source). **Note**: **Android-only**; older project (last activity years ago); not for iOS . **Best for**: teams with physical Android devices wanting browser-based remote control .



**Frameworks for building custom systems**: Combine **tapflow** for browser-based simulator sharing with **dockerify-android** for headless Android emulation and **TouchHLE** or **LightTouch** for classic iOS apps—creating a layered open-source mobile emulation stack. **None match Corellium's full iOS virtualization or BrowserStack's real-device parity**, but for simulator/emulator-based testing, the options are production-capable.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Mobile emulation platforms handling app binaries and test data must comply with data protection regulations (GDPR, CCPA, etc.) and app store policies.

- **The "real device farm" vs. "simulator/emulator streaming" vs. "local emulator" vs. "classic iOS emulation" distinction is critical.** **BrowserStack, Sauce Labs, LambdaTest, and Genymotion Cloud** are **real device/cloud farms**—they provide real hardware or managed emulators . **tapflow and GADS** are **self-hosted simulator/emulator streaming**—they share your own Macs' simulators via browser . **dockerify-android and NixDroid** are **local emulators**—they run on your machine . **TouchHLE and LightTouch** are **classic iOS emulation**—they run legacy apps without Apple hardware . **Choose based on whether you need real devices, shared simulators, local emulation, or legacy app support.**

- **tapflow is the most complete self-hosted simulator streaming platform**—browser access, H.264 streaming, MCP server, and session recordings . **The trade-off**: macOS-only agents; not a device farm; no Appium integration.

- **GADS is the most complete self-hosted device farm**—Appium integration, WebRTC streaming, and remote control . **The trade-off**: proprietary hub-ui; iOS requires Xcode.

- **TouchHLE and LightTouch are for classic apps only**—32-bit iPhone OS 2.x/3.0 era; not for modern 64-bit apps . **Do not evaluate for current iOS testing.**

- **Corellium is the only full iOS virtualization**—but it is quote-only, complex, and Linux/Mac only . **For security research, it is the benchmark** .

- Self-hosted open-source solutions require proper setup (macOS for tapflow, Docker/KVM for dockerify-android, Appium for GADS). **Emulators handle app binaries and test data**—ensure your deployment meets your organization's security and compliance requirements before processing production builds.



---



**Made for mobile developers, QA engineers, and organizations building transparent emulation solutions.**

Let's make Android & iOS Emulators and Simulators more open, data-driven, and device-accessible.
