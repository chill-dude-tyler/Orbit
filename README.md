# Orbit 🪐

**A screen-time and focus companion built for students, not against them.**

Orbit helps students aged 11–25 build healthier digital habits without feeling
policed. Instead of acting as a blunt blocker, it pairs smart scroll-time
limits with real productivity tools — so students actually want to use it,
not just tolerate it.

---

## Why Orbit

Most screen-time apps either do nothing or feel like a lockdown. Orbit tries
a middle path: fair limits, clear warnings, a way to negotiate more time when
it's genuinely needed, and tools that actually help students focus — not just
apps that stop them from scrolling.

## Features

**Scroll & limit detection**
- Detects scrolling in real time using Android's Accessibility Service
- Daily limits start as smart suggestions based on a student's first week of
  usage, then get fine-tuned by a parent/guardian
- Warnings at 10, 5, and 1 minute before a limit hits — never a sudden cutoff
- Minimal lock screen when time runs out, with a clear path back to focus

**Fair bypass system**
- One bypass request per day, made from inside the app
- Parent approves remotely and grants bonus minutes via a simple time picker
- Offline-first — works without an internet connection

**Focus tools**
- One-tap Focus Mode to block distracting apps during a study session
- Built-in Pomodoro timer
- Notes organizer with note-to-task conversion

**Personalization**
- Light, dark, and fully custom theme creator
- Font customization
- GitHub-style habit-streak calendar

**For parents**
- Weekly reports comparing study time vs. scroll time
- Gentle weekly check-in prompts
- Parent Mode for adjusting limits and reviewing activity

## Tech stack

- **Language:** Kotlin
- **UI:** Jetpack Compose, Material Design 3
- **Architecture:** MVVM
- **Persistence:** Room (structured data), DataStore (preferences/flags)
- **Background work:** WorkManager (daily resets, weekly reports)
- **Security:** bcrypt password hashing for guardian credentials
- **System integration:** AccessibilityService, DevicePolicyManager,
  UsageStatsManager — no camera, no invasive tracking
- **CI/CD:** GitHub Actions builds and packages the APK on every push

## Project status

Actively in development ahead of the Spark '26 working-build deadline.
Core architecture (navigation, database, theming, service scaffolding) is in
place; screen implementations and detection/enforcement logic are in progress.

## Developer

Built by **chill-dude-tyler** Real name **Sanul Sandira** at ***Royal College***

GitHub: [github.com/chill-dude-tyler](https://github.com/chill-dude-tyler)
