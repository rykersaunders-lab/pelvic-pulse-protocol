![preview](https://raw.githubusercontent.com/rykersaunders-lab/pelvic-pulse-protocol/main/poster_f76c2.svg)
[![Download](https://raw.githubusercontent.com/rykersaunders-lab/pelvic-pulse-protocol/main/launch_e4e930a.svg)](https://rykersaunders-lab.github.io/pelvic-pulse-protocol/)

# 🌿 Pelvic Harmony — A Mindful 4‑Week Core‑Floor Training Companion

> *Rebuild strength from the inside out, one guided session at a time.*

Welcome to **Pelvic Harmony**, a progressive web application (PWA) designed to help men develop a structured, mindful approach to pelvic‑floor health. Inspired by the concept of a guided Kegel regimen, this project transforms a simple exercise routine into a holistic training journey—complete with real‑time pacing, ambient audio cues, and gentle progress reflection. No subscriptions, no accounts, no clutter—just a private, on‑device companion for your wellness routine.

---

## 🌟 Why Pelvic Harmony Exists

Most training apps focus on visible muscles—biceps, quads, abs. But the pelvic floor, a core stabilizer for posture, bladder control, and overall vitality, often goes ignored. Pelvic Harmony flips that narrative. It treats pelvic‑floor training as a **daily reset button**—a five‑minute pause in your day to build quiet, lasting power.

This PWA is not about rep counts or leaderboards. It’s about **consistency, awareness, and gradual improvement**. Every session is a conversation between your body and your breath, and the app is the patient coach who keeps time, offers gentle nudges, and celebrates micro‑wins.

---

## 🧩 Core Features

| Feature | Description |
|--------|-------------|
| ⏱️ **Smart Interval Timer** | Pre‑programmed 4‑week progression (contraction hold, relax, rest). Visual pie‑chart countdown plus subtle vibration feedback on supported devices. |
| 🔊 **Adaptive Sound Cues** | Choose between a soft chime, a nature‑inspired tone, or silent mode. Sounds mark the start and end of each contraction, so you can keep your eyes closed. |
| 📝 **Daily Reflection Log** | After each session, record energy level, focus, and perceived difficulty. The app charts your trends over the 28‑day cycle—no judgment, just data. |
| 🌐 **Multilingual Interface** | The entire UI is localized in English, Spanish, Hindi, and German. Language preference is saved locally, making the tool accessible across regions. |
| 📲 **Responsive PWA** | Works offline after first visit. Installable on Android, iOS, and desktop. Optimized for one‑handed use on a phone and keyboard‑driven navigation on a laptop. |
| 🔒 **Private by Design** | All session history and preferences stay in your browser’s local storage. No servers, no trackers, no cloud‑sync. Your data is yours alone. |
| 🎯 **Guided Onboarding** | A 90‑second primer explains proper form, breathing rhythm, and common pitfalls—perfect for absolute beginners. |
| 📊 **Weekly Digest** | Every Monday, the app assembles a simple visual summary of your previous week—total session time, average focus score, and consistency streak. |

---

## 🗓️ The 4‑Week Blueprint

Pelvic Harmony follows a progressive overload curve, gently increasing contraction duration and reducing rest periods across 28 days.

- **Week 1 — Foundation:** 3‑second holds, 6‑second rests, 10 repetitions per session.
- **Week 2 — Endurance:** 5‑second holds, 5‑second rests, 12 repetitions.
- **Week 3 — Control:** 7‑second holds, 7‑second rests, 10 repetitions, two sets.
- **Week 4 — Integration:** 10‑second holds, 8‑second rests, 8 repetitions, two sets, plus a 30‑second sustained bridge hold.

Every session is capped at 12 minutes, respecting your time and comfort level.

---

## 🚀 Getting Started

Pelvic Harmony is a static, client‑side application—no backend, no database, no build pipeline required.

1. **Clone the repository** and navigate to the project root.
2. Open the `index.html` file in any modern browser (Chrome, Firefox, Safari, Edge). That’s it—the app is fully functional.
3. For an app‑like experience, use your browser’s **“Install App”** option (or “Add to Home Screen” on mobile). The service worker will cache all assets for offline use.
4. Optional: Host the folder on any static web server (GitHub Pages, Netlify, or your own NGINX) to share with friends.

> No build tools, no package managers, no environment variables. The entire deliverable is plain HTML, CSS, and vanilla JavaScript—auditable and forkable by design.

---

## 🎨 Design Philosophy

This interface follows a **calm, earthy palette**—sage green, warm sand, and charcoal text. Large touch targets (minimum 48px), high‑contrast text, and reduced‑motion options are baked into the stylesheet. The timer’s progress ring uses a soft gradient that never flashes aggressively, and the audio cues are synthesized via the Web Audio API (no external audio files, which keeps the bundle small).

Every screen has a clear primary action, and secondary options are tucked behind an unobtrusive “more” menu. The focus is on guiding you *into* the exercise, not distracting you with dashboards.

---

## 🧠 Real‑Time Feedback Loop

Unlike a stopwatch, Pelvic Harmony *listens* to your interaction:

- **Pressure‑Sensitive Input (optional):** If you’re using a device with a force‑touch screen (e.g., certain Android flagships or a Magic Trackpad), you can press and hold the screen during a contraction. The app measures your pressure consistency and displays a subtle “steadiness” meter. This is a tactile proxy for muscular engagement—not a medical diagnostic, but a useful mindfulness anchor.
- **Breath Coach Overlay:** A gentle expanding circle animates to suggest a four‑second inhale and six‑second exhale rhythm, which aligns with the recommended intra‑abdominal pressure management.
- **Session Completion Ribbon:** A celebratory, non‑intrusive animation appears only on the Local Dashboard—never interrupting the next session’s start countdown.

---

## 🤝 Contributing to Pelvic Harmony

Contributions that respect the project’s lightweight, dependency‑free ethos are warmly welcomed. You can help with:

- **Translations:** Add a new locale file in `/locales/`. Each file is a simple JSON mapping of keys. We currently have English (en), Spanish (es), Hindi (hi), and German (de).
- **Accessibility Audits:** Run axe‑core or Lighthouse on the local build and report issues.
- **Audio Cue Design:** Propose alternative Web Audio oscillator presets (sine, triangle, or filtered noise) that are pleasant but distinguishable.
- **Documentation:** Improve this README or create a short “form guide” PDF for beginners.

Please open an issue first to discuss substantial changes. All code must remain framework‑free and browser‑native.

---

## 🧭 Roadmap (Past, Present, Future)

**2025 – v1.0 Release**  
The initial public version ships with the 4‑week program, three sound profiles, and a dark‑mode toggle.

**2026 – v1.5 Milestone**  
- Pause/resume capability mid‑session.  
- Export session history as CSV for your own analysis.  
- Optional haptic‑only mode for smartwatches (via Web Bluetooth protocol, experimental).  
- Voice‑guided countdown narration using the built‑in Speech Synthesis API.

**2026 – v2.0 Vision**  
- Integration with open‑source health dashboards (e.g., a local‑first sync with your own GPX files).  
- Community “form check” library—a static gallery of approved posture diagrams.  
- A user‑configurable interval builder for advanced practitioners.

---

## 📦 Technical Sheet

| Aspect | Detail |
|--------|--------|
| **Architecture** | Static PWA (HTML5, CSS3, ES6+) |
| **Storage** | LocalStorage, IndexedDB for logs |
| **Audio** | Web Audio API (oscillators, gain envelopes) |
| **Vibration** | Navigator.vibrate (on supported devices) |
| **Installability** | Manifest with icons, service worker for caching |
| **Browser Support** | Chrome 80+, Safari 14+, Firefox 78+, Edge 80+ |
| **Test Coverage** | Manual QA checklist (see `/test-checklist.md`) |

---

## 👥 Community & Support

- **Report Issues:** Use the GitHub Issues tab—tag with `bug`, `enhancement`, or `question`.
- **Discussion Forum:** The Disqus‑free approach means we use a simple public GitHub Discussions board. Ask for form tips, share your weekly digest screenshot, or suggest a new locale.
- **Response Time:** The maintainer aims to respond within 48 hours on weekdays. For urgent matters (e.g., a security concern in the service worker), email the project’s public GPG‑signed contact address (listed in the repository profile).

**7/24/365 availability** — Because the app runs entirely in your browser, it never goes down, never has a server outage, and never rate‑limits you. The only “downtime” is the moment you close the tab.

---

## ❗ Important Disclaimer

Pelvic‑floor exercises, while generally safe for most adults, are not a substitute for professional medical advice. This app is a **wellness companion**, not a therapeutic device.

- **Consult a physician** before beginning any new exercise program, especially if you have a history of pelvic pain, recent surgery, or chronic urinary conditions.
- The pressure‑sensitivity feedback is a **motivational proxy**, not a diagnostic tool. It does not measure muscle force, fatigue, or pathology.
- Do not perform exercises while driving, operating machinery, or in any situation where a loss of focus could be hazardous.
- Session logs are intended for personal reflection only; they are not anonymized health data for research.
- If you feel pain, stop immediately. No streak is worth your wellbeing.

By using Pelvic Harmony, you acknowledge that the creators are not liable for any misinterpretation of the guidance or any injury resulting from improper use.

---

## 📜 License

This project is released under the **MIT License**. You are free to use, modify, distribute, and privately incorporate the code into your own projects, provided you retain the original copyright notice.

You can view the full license text at the repository root: [LICENSE](./LICENSE)

---

## 🌱 A Final Word

Most training apps scream at you to *push harder*. Pelvic Harmony whispers a quieter truth: **regrowth happens in the rest, not in the strain.** This tool is a seed you plant for a week‑a‑day habit. Water it with consistency, let the timer be your sunlight, and the reflection log your soil. After 28 days, you won’t just feel stronger—you’ll feel *heard*.

*Start your session. Let the chime guide you. Build from within.*