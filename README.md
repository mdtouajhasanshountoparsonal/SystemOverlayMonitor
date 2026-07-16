# System Overlay Monitor

Real-time typing overlay with mesh particles, WPM tracking, hacker glitch effects, and word match detection. Your keystrokes, visualized.

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyQt6](https://img.shields.io/badge/PyQt6-GUI-41CD52?style=for-the-badge&logo=qt&logoColor=white)
![PyInstaller](https://img.shields.io/badge/PyInstaller-EXE-000000?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

---

## Features

- **Real-Time WPM Tracking** — Live words-per-minute calculation using a 12-second sliding window
- **Mesh Particle Animation** — Cyan + purple particles with connection lines and lightning bolts
- **Hacker Glitch Overlay** — Full-screen scanlines, random characters, RGB channel split on word match
- **Smoke Effect** — New words rise upward like smoke and fade out
- **Flash Overlay** — Full-screen color flash (red for special, green for repeated words)
- **Screen Shake** — Window shakes on word match with random offsets
- **Particle Explosion** — Burst of particles from center on word match
- **Ghost Typing** — Shows your current keystrokes in real-time on the overlay
- **Word Match Detection** — Compares typed words against SQLite database for repeats
- **Special Word Triggers** — Custom words trigger enhanced effects
- **Click-Through Mode** — Minimized 250x110px overlay that doesn't block input
- **Welcome Splash** — Matrix rain + glitch text animation on startup
- **App Usage Monitoring** — Tracks application usage time with alerts
- **Settings Panel** — Toggle every effect on/off from the tray menu
- **Crash Logger** — Automatic error logging to crash.log

## Screenshots

| Full Mode | Minimized Mode | Login Screen |
|-----------|---------------|--------------|
| Full overlay with WPM, ghost typing, mesh background | Compact click-through panel | Password-protected entry |

## Installation

### Download (Recommended)

1. Go to [Releases](https://github.com/mdtouajhasanshountoparsonal/SystemOverlayMonitor/releases)
2. Download `SystemOverlayMonitor.exe`
3. Double-click to run — no installation needed

### Build from Source

```bash
# Clone the repository
git clone https://github.com/mdtouajhasanshountoparsonal/SystemOverlayMonitor.git
cd SystemOverlayMonitor

# Install dependencies
pip install PyQt6 pyinstaller

# Build single-file EXE
pyinstaller --onefile --windowed --icon=icon.ico main.py
```

## Usage

1. Run `SystemOverlayMonitor.exe`
2. Login with your credentials
3. The overlay appears on your screen
4. Start typing — watch mesh particles react to your keystrokes
5. Right-click the tray icon to access settings

## Tech Stack

| Technology | Purpose |
|-----------|---------|
| Python 3.x | Core language |
| PyQt6 | GUI framework |
| PyInstaller | Single-file EXE builder |
| SQLite | Local database |
| QMediaPlayer | Sound effects |
| QPropertyAnimation | Smooth animations |

## Settings

Open the settings panel from the system tray menu to toggle:

- Mesh Particles
- Hacker Glitch
- Smoke Effect
- Screen Shake
- Particle Explosion
- Sound Effects
- Ghost Typing
- Mesh Overlay (on word match)

## Database

SQLite database is stored at:
```
%LOCALAPPDATA%\SystemOverlayMonitor\monitor_data.db
```

Tracks:
- Typed words (for word match detection)
- Special trigger words
- App usage statistics
- User settings

## License

MIT License - see [LICENSE](LICENSE) for details.

## Author

**THS** — [GitHub](https://github.com/mdtouajhasanshountoparsonal)

---

*Built with Python + PyQt6*
