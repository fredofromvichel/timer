# ⏱️ Countdown Timer – Extended Version

A modular, presentation‑ready and fully client‑side countdown timer. Created with AI support.

## 🚀 Overview
This project provides a highly customizable countdown timer built entirely with vanilla HTML, CSS, and JavaScript. It is optimized for presentations, workshops, meetings, and live events.

## ✨ Features
- Start / Stop / Reset controls
- Stable, non-jumping time display (fixed-width digits, centered colon)
- Configurable visual + audio signal before 0:00 (off / 1 / 2 / 3 / 5×)
- Optional continuation into negative time (e.g., -0:12)
- Size presets and manual scaling via keyboard (+ / -)
- Timer-only visibility toggle — hides the countdown while controls stay visible (key: B)
- UI that auto-contrasts to the chosen background color (readable on light and dark)
- Fullscreen mode (key: F)
- UI dimming while the timer is running
- Live-updating URL parameters for sharing configurations
- Comprehensive keyboard shortcuts

## 🔗 URL Parameters
- `min` – start minutes
- `size` – small / medium / large
- `lz` – leading zero
- `blink` – number of visual blinks before 0:00 (0/1/2/3/5); also controls the 0:00 sound (0 = silent)
- `fg` / `bg` – colors
- `font` – font family alias
- `settings` – 0/1 to show settings panel
- `neg` – allow negative time
- `autostart` – automatically start timer

## ⌨ Keyboard Shortcuts
| Key | Function |
|-----|----------|
| Space | Start / Stop |
| R | Reset |
| F | Toggle fullscreen |
| B | Toggle timer visibility |
| + / - | Scale timer size |
| ESC | Close settings panel |

## 🧩 Architecture
### State Management
- `remainingMs`, `endAt`, `running`, `finished`
- `timerScale` for zooming
- `timerHidden` for visibility toggle
- `allowNegative` for negative time continuation

### Core Functions
- `start()`, `stop()`, `reset()`
- `tick()` — frame-based loop via `requestAnimationFrame`
- `formatTimeParts()` / `formatTime()` — split mm / ss for a stable, fixed-width display, including negative time
- `applyTheme()` — applies colors/font and derives the auto-contrasting UI chrome from the background
- `applySizePreset()`
- `syncUrl()`, `applyFromUrl()` for shareable URLs

## 📄 License
```
Countdown Timer – Extended Version
Copyright (c) 2026 Frederic Krone

MIT License (Attribution required)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, subject to the following conditions:

- This copyright notice must be included in all copies.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

# ⏱️ Countdown Timer – Extended Version

Modularer, erweiterbarer und präsentationstauglicher Web‑Timer. Mithilfe von KI erstellt.

## 🚀 Überblick
Dieses Projekt ist ein vollständig clientseitiger, hochgradig konfigurierbarer Countdown‑Timer für Präsentationen, Workshops und Live‑Events.

## ✨ Features
- Start / Stop / Reset
- Ruhige, springfreie Zeitanzeige (gleich breite Ziffern, zentrierter Doppelpunkt)
- Konfigurierbares visuelles + akustisches Signal vor 0:00 (Aus / 1 / 2 / 3 / 5×)
- Optionales Weiterlaufen in die negative Zeit (z. B. -0:12)
- Schriftgrößen-Presets und frei skalierbare Anzeige (+ / -)
- Unsichtbarkeitsmodus: blendet nur den Timer aus, Bedienelemente bleiben sichtbar (Taste: B)
- Bedienoberfläche, die sich automatisch an die Hintergrundfarbe anpasst (hell wie dunkel lesbar)
- Vollbildmodus (Taste: F)
- UI-Dimming während der Laufzeit
- Dynamische URL‑Parameter zur Weitergabe der Einstellungen
- Umfassende Tastatur‑Shortcuts

## 🔗 URL-Parameter
- `min` – Startminuten
- `size` – small / medium / large
- `lz` – führende Null
- `blink` – Anzahl visueller Blinks vor 0:00 (0/1/2/3/5); steuert auch den Ton bei 0:00 (0 = stumm)
- `fg` / `bg` – Farben
- `font` – Schriftart
- `settings` – 0/1 für Panelstatus
- `neg` – negative Zeit erlauben
- `autostart` – Timer automatisch starten

## 📄 Lizenz
```
Countdown Timer – Extended Version
Copyright (c) 2026 Frederic Krone

MIT License (Attribution required)

Hiermit wird jedem kostenlos die Erlaubnis erteilt, dieses Skript
zu verwenden, zu kopieren, zu verändern und weiterzugeben – auch
kommerziell –, unter der Bedingung, dass folgende Hinweise enthalten bleiben:

- Diese Copyright-Notiz

Das Skript wird ohne Gewährleistung bereitgestellt – ohne Anspruch
auf Funktion, Eignung oder Fehlerfreiheit.
```

