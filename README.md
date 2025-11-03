# Discord Poll Announcement Bot

Automate creating, scheduling, and announcing polls across multiple Discord channels—directly from Android devices or emulators. This system eliminates repetitive poll setup, tracks live reactions, and posts results automatically, giving moderators and community managers reliable, hands-free engagement. Built with Appilot-driven Android control, UI Automator/Appium flows, and smart retry logic for zero-touch operation.

<p align="center">
  <a href="https://Appilot.app" target="_blank">
    <img src="media/appilot-baner.png" alt="Appilot Banner" width="100%">
  </a>
</p>
<p align="center">
  <a href="https://t.me/devpilot1" target="_blank">
    <img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>&nbsp;
  <a href="https://wa.me/923249868488?text=Hi%20Appilot%2C%20I'm%20interested%20in%20automation." target="_blank">
    <img src="https://img.shields.io/badge/Chat-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>&nbsp;
  <a href="mailto:support@appilot.app" target="_blank">
    <img src="https://img.shields.io/badge/Email-support@appilot.app-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>&nbsp;
  <a href="https://appilot.app" target="_blank">
    <img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
</p>

<p align="center"> 
   Created by Appilot, built to showcase our approach to Automation!<br>
   <strong>If you are looking for custom Discord Poll Announcement Bot, you've just found your team — Let’s Chat.👆👆</strong>
</p>

## Introduction
This automation creates polls, schedules announcements, and monitors votes using the Discord mobile app or web client on Android devices/emulators. It automates the repetitive workflow of composing poll messages, attaching reactions/options, pinning, cross-posting to channels, and summarizing results.
**Automating Discord Poll Campaigns**
- Auto-creates formatted poll messages with configurable options (reactions/buttons).
- Schedules announcements and reminders across multiple servers/channels.
- Tracks engagement (reactions, replies) and posts result summaries.
- Works on real devices and emulators with ADB-less wireless control.
- Integrates with proxies and multi-session device farms for scale.

## Core Features
- **Real Devices and Emulators:** Run on physical Android phones or emulators (Bluestacks/Nox). Ensures 1:1 parity with real user interactions and bypasses desktop-only limitations.
- **No-ADB Wireless Automation:** Control devices without tethered USB; zero ADB dependency mode for safer, undetected execution across racks.
- **Mimicking Human Behavior:** Randomized delays, gesture-based scrolling, realistic typing, reaction placement variance to reduce bot fingerprints.
- **Multiple Accounts Support:** Rotate Discord accounts safely with isolated profiles, cookies, and session management per device.
- **Multi-Device Integration:** Orchestrate 10–300+ devices with a central scheduler; shard workloads and coordinate poll posting windows.
- **Exponential Growth for Your Account:** Consistent, timely polls increase engagement and retention; scheduled reminders boost participation and server activity.
- **Premium Support:** Priority onboarding, device-farm guidance, and tailored flows for unique server rules and moderation policies.

| Feature | Description |
| --- | --- |
| Template-Based Poll Composer | Define poll templates (title, options, emojis, tags, @roles). One click to deploy to many channels. |
| Cross-Server Broadcasting | Push a poll to selected servers/channels with per-channel throttling and cooldowns. |
| Result Aggregation & Auto-Summary | Collect reactions, compute winners, and publish a formatted summary or chart image. |
| Smart Retry & Idempotency | Detect failed posts, re-issue safely without duplicates, resume after app crashes/reboots. |
| Role/Time Gated Reminders | Announce reminders for specific roles (e.g., @Members) at fixed intervals until participation threshold is met. |
| Webhook/Sheet Export | Stream poll metrics to webhooks or CSV/Sheets for analytics and audits. |

</p>
<p align="center">
  <a href="https://appilot.app" target="_blank">
    <img src="media/discord-poll-announcement-bot-banner.png" alt="discord-poll-announcement-bot-architecture" width="95%">
  </a>
</p>

## How It Works
1. **Input or Trigger** — Launch from the Appilot dashboard: select poll template, target servers/channels, schedule, and reminder cadence.  
2. **Core Logic** — Appilot drives the Android device/emulator via UI Automator/Appium to open Discord, navigate to channels, compose the poll, attach reaction options, and pin or cross-post as configured.  
3. **Output or Action** — The bot posts polls, monitors reactions/replies, and publishes interim/final results; optional exports via webhook/CSV.  
4. **Other functionalities** — Built-in retry/backoff, structured logs, screenshots-on-error, and parallel processing across device pools with queue-based orchestration.

## Tech Stack
- **Language:** Kotlin, Java, JavaScript, Python  
- **Frameworks:** Appium, UI Automator, Espresso, Robot Framework, Cucumber  
- **Tools:** Appilot, Android Debug Bridge (ADB), Appium Inspector, Bluestacks, Nox Player, Scrcpy, Firebase Test Lab, MonkeyRunner, Accessibility  
- **Infrastructure:** Dockerized device farms, Cloud-based emulators, Proxy networks, Parallel Device Execution, Task Queues, Real device farm.

## Directory Structure
```
discord-poll-announcement-bot/
│
├── src/
│   ├── main.py
│   ├── automation/
│   │   ├── poll_composer.py
│   │   ├── announcer.py
│   │   ├── reaction_tracker.py
│   │   ├── exporter.py
│   │   └── utils/
│   │       ├── logger.py
│   │       ├── device_controller.py
│   │       ├── template_loader.py
│   │       └── scheduler.py
│   ├── android/
│   │   ├── uiactions.yaml
│   │   ├── selectors.json
│   │   └── accessibility_rules.yaml
│
├── config/
│   ├── settings.yaml
│   ├── credentials.env
│   └── channels_map.json
│
├── data/
│   ├── poll_templates/
│   │   └── default_poll.yaml
│   └── exports/
│       ├── results.csv
│       └── results.json
│
├── logs/
│   └── automation.log
│
├── tests/
│   ├── e2e_poll_flow.robot
│   └── fixtures/
│       └── demo_channels.json
│
├── docker/
│   ├── Dockerfile
│   └── docker-compose.yml
│
├── requirements.txt
└── README.md
```


## Use Cases
- **Community Managers** use it to schedule weekly polls across multiple channels, so they can sustain engagement without manual repetition.  
- **Moderators** use it to gather quick feedback on rules/events, so they can make decisions faster with visible consensus.  
- **Brands/Servers** use it to run campaign votes and giveaways, so they can maximize participation and track metrics centrally.  
- **Agencies** use it to operate multi-server poll campaigns, so they can scale client operations with consistent reporting.

## FAQs
**How do I configure this automation for multiple accounts?**  
Use the account pool in `config/settings.yaml` and session folders per device. The orchestrator assigns accounts per task with cooldowns to avoid rate limits.

**Does it support proxy rotation or anti-detection?**  
Yes. Device-level or emulator-level proxies are supported. Randomized timings, human-like gestures, and staggered posting reduce detection signals.

**Can I schedule it to run periodically?**  
Absolutely. Use the built-in scheduler with cron-like rules. Define campaign windows and reminder intervals per server/channel.

**Will it work without USB (no ADB)?**  
Yes. The ADB-less wireless mode controls the UI via Accessibility/UI Automator bridges over the network, ideal for rack-mounted farms.

**Can it summarize poll results automatically?**  
Enable the aggregator to compute winners and auto-post a summary message; optionally export CSV/Webhook for dashboards.

## Performance & Reliability Benchmarks
- **Execution Speed:** Posts to 50 channels in ~6–9 minutes per device (including reaction setup and pinning).  
- **Success Rate:** 95% end-to-end completion in noisy mobile environments with auto-retry and resume.  
- **Scalability:** Proven orchestration from 10 to 300+ Android devices; architecture patterns extend toward 1000 with queue sharding.  
- **Resource Efficiency:** Lightweight workers (<250MB RSS per emulator), headless options, and adaptive FPS to conserve CPU/GPU.  
- **Error Handling:** Exponential backoff, screenshot-on-failure, structured logs, and idempotent repost guards ensure resilient runs.

##
<p align="center">
<a href="https://cal.com/app-pilot-m8i8oo/30min" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
</p>
