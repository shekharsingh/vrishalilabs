<img src="icon.png" width="96" alt="Rojana Planner icon">

# Rojana Planner

**A complete yearly, monthly, weekly and daily planner for Android — by Vrishali Labs.**

Rojana (रोज़ाना, "every day") gives you a full paper-style planner on your phone, tablet or foldable:
plan the year, break it into quarters, months and weeks, and run each day with a schedule, top priorities,
notes and a reflection page. An optional journal waits at the end of every day.

## Features

| Page | What you can do |
|---|---|
| **Year** | 12 mini calendars with ISO week numbers. Tap any month, week number or day to open it. Year notes. |
| **Quarter (Q1–Q4)** | Three months at a glance plus quarter notes for goals and reviews. |
| **Month** | Month grid with a writable box for every date (tap the date to open the day). Month notes. |
| **Week** | Seven day boxes (Monday–Sunday) plus week notes; shows priority progress and journal days. |
| **Day — Plan** | Hour-by-hour schedule (default 07:00–23:00, adjustable), 8 top priorities with tick-off, notes. |
| **Day — More notes** | A full extra notes page for the day. |
| **Day — Reflect** | Things I'm grateful for · The best thing that happened today · Daily log. |
| **Day — Journal (optional)** | Stays a simple offer until you start it. One entry per date: title, mood and text. Can be removed any time. |
| **Notes Index** | 105 numbered notes on three index pages, per year. |

Also:

- **Multiple years** — 2026 onwards; pick a year at the top, add more years whenever you need them.
- Page tabs (Year › Quarter › Month › Week › Day), ‹ › buttons and swipe for previous/next page, **Today** button.
- **Search** across everything you have written; list of all journal entries.
- Light, dark or system theme; layouts adapt to phones, tablets and unfolded foldables.
- **Private by design** — no account, no ads, no analytics, no internet permission. Everything stays on your device.
  Export/import a backup file whenever you like.

Requires Android 8.0 (API 26) or newer.

## Privacy

Rojana Planner does not collect or share any personal data. See the
[privacy policy](https://shekharsingh.github.io/vrishalilabs/rojanaplanner/privacy.html) ([source](privacy.html)).

## Building

1. Open the project in Android Studio (AGP 8.13, Kotlin 2.2, Gradle 8.14, JDK 17+).
2. Run the `app` configuration, or `gradlew assembleDebug`.
3. Unit tests: `gradlew testDebugUnitTest`.
4. Release: put your upload-key details in `keystore.properties` (never commit it), then `gradlew bundleRelease`.

```
storeFile=keystore/rojana-upload.jks
storePassword=…
keyAlias=rojana
keyPassword=…
```

The app uses only the Android framework and the Kotlin standard library — no third-party dependencies.

### Code map

```
app/src/main/java/com/vrishalilabs/rojanaplanner/
  core/   calendar maths, pages & navigation, storage keys, repository, backup format (pure Kotlin, unit-tested)
  data/   SQLite storage
  ui/     activity, pages, mini-month calendar, paper-style editors
app/src/test/   unit tests
```

## Support

support@vrishalilabs.com

## License

Copyright © 2026 Vrishali Labs. All rights reserved. See [LICENSE](LICENSE).
