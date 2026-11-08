# Awesome-Android-IOS-Emulators-And-Simulators

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

- **BrowserStack**
  **Cloud device farm** with real devices and emulators. **Pricing**: **Desktop & Mobile plans**; App Live from ~$39/month; App Automate from ~$199/month. **Free tier**: Open-source free; trial available. **Best for**: teams wanting real-device parity for mobile testing—**trade-off**: costs scale with parallel sessions; emulator-only testing is cheaper.

- **Sauce Labs**
  **Cloud testing platform** with emulators and real devices. **Pricing**: **Live Testing from $199/month**; **Automated Testing from $199/month**; Enterprise custom. **Free tier**: Free trial; free tier for open-source. **Best for**: enterprises needing both emulators and real devices with strong security—**trade-off**: inflexible pricing noted by reviewers.

- **LambdaTest**
  **Cloud testing** with virtual devices and real devices. **Pricing**: **Virtual Devices** included in plans; **Real Devices** add-on. **Free tier**: Limited free plan. **Best for**: teams wanting affordable access to both emulators and real devices—**trade-off**: real devices cost extra.

- **Genymotion Cloud**
  **Android emulator in the cloud**. **Pricing**: **SaaS from $0.05/minute**; **On-premise** available. **Free tier**: Trial available. **Best for**: teams wanting Android-only cloud emulation with API access—**trade-off**: Android-only; no iOS support.

- **Appetize.io**
  **Browser-based mobile app streaming**. **Pricing**: **Free tier** with limited minutes; **paid from ~$40/month**. **Free tier**: Yes, limited. **Best for**: sharing app builds via browser without device setup—**trade-off**: not a full testing platform; streaming-focused.

- **Corellium**
  **Full iOS virtualization** for security research. **Pricing**: **Quote-only**; enterprise contracts. **Free tier**: Trial available upon request. **Best for**: security researchers needing full iOS device emulation (ARM-based)—**trade-off**: complex setup; Linux/Mac only, not Windows .

- **Android Studio AVD**
  **Official Android emulator** bundled with Android Studio. **Pricing**: Free. **Free tier**: Yes. **Best for**: Android developers wanting the official, well-supported emulator—**trade-off**: resource-heavy; no iOS support.

- **Xcode Simulator**
  **Official iOS simulator** bundled with Xcode. **Pricing**: Free with Apple ID. **Free tier**: Yes. **Best for**: iOS developers on macOS wanting the most accurate simulator—**trade-off**: macOS-only; 12GB+ install .

- **BlueStacks**
  **Consumer Android emulator** for gaming. **Pricing**: Free with ads; premium subscription. **Free tier**: Yes. **Best for**: consumers running Android games on PC—**not for development/testing**.

- **NoxPlayer**
  **Consumer Android emulator** for gaming. **Pricing**: Free. **Free tier**: Yes. **Best for**: consumers running Android games on PC—**not for development/testing**.

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
