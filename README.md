## Andrei Leganov — Senior iOS Engineer

[Русская версия](README.ru.md)

Paphos, Cyprus · 7 years of commercial Swift.
I build consumer apps end-to-end: architecture → implementation → App Store release.

**Shipped**
- [Doers United](https://apps.apple.com/cy/app/doers-united/id6747444014) — professional networking app with AI matchmaking, events and real-time chat, built from scratch as the sole iOS engineer
- [Anymaster](https://apps.apple.com/cy/app/anymaster-services-near-you/id6444522591) — local services marketplace, built from scratch as the sole iOS engineer
- [Webasyst Cash Flow & Forecast](https://apps.apple.com/cy/app/webasyst-cash-flow-forecast/id6450029747) — cash-flow tracking and forecasting for small businesses
- [Blink](https://apps.apple.com/cy/app/blink-friends-location/id1668580784) — friends map and messenger; later relaunch of a product whose core I wrote with another iOS engineer

**Building with agents**

Over the past year I've been writing tools for working with coding agents, and writing them with agents. What I took away: reliability doesn't come from a better prompt — it comes from the constraints around the agent, the checks that run without a human.

- **[threadcode](https://github.com/andreileganov/threadcode)** — a desktop client (macOS, Electron) where a conversation branches into threads like in Slack. A thread inherits the full parent context, nothing leaks back, and both panes run at once. Each thread gets its own git worktree and branch, so its edits never touch the main work. Isolation is proven by live runs against the real SDK, not mocks: a code word given to the parent showed up in the thread; a word only the thread knew stayed unknown to the parent. Source is public: 70 commits, 23 test files, ~8,700 lines.
- **Harness before code.** Hooks block commits to `main`, writes outside the project and reads of `.env`. Every request carries the current branch, uncommitted files and the acceptance criteria still open. A quality gate runs on stop: types, linter, tests.
- **On spec-driven work.** A test written after the code, from the code, only proves the code does what it does. A test written from an acceptance criterion proves it does what was promised. The files look the same; the meaning is the opposite.
- **A personal agent** on Claude Code running on a server: tasks, calendar, notes. The interesting part isn't the features but the twelve hooks that stop it from breaking its own rules — including one that forbids claiming something doesn't exist until a primary source has been checked. Every tool ships with a self-check, and one run verifies them all.

**Stack**
Swift · UIKit · SwiftUI · SnapKit · Combine · async/await · actors · MVVM + Coordinator · VIPER · StoreKit · GitLab CI/CD

**Elsewhere**
[LinkedIn](https://www.linkedin.com/in/andreileganov) · arickpost@gmail.com · Telegram [@arickxic](https://t.me/arickxic) · [CV (PDF)](Andrei_Leganov_iOS_CV.pdf)

---

Most of my production code lives in private repositories.
