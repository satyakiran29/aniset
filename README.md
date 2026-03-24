<p align="center">
  <h1 align="center">🎌 Aniset — Anime KWGT Widgets</h1>
  <p align="center">
    Beautiful anime-themed KWGT widgets, wallpapers & ringtones for your Android home screen.<br/>
    Also the asset backend for upcoming <strong>Aniset Pro</strong> and <strong>Anify</strong>.
  </p>
</p>

<p align="center">
  <a href="https://play.google.com/store/apps/details?id=com.skdev.aniset">
    <img src="https://img.shields.io/badge/Google%20Play-Download-green?style=for-the-badge&logo=google-play" alt="Google Play" />
  </a>
  <a href="https://aniset.vercel.app/">
    <img src="https://img.shields.io/badge/Website-aniset.vercel.app-blue?style=for-the-badge&logo=vercel" alt="Website" />
  </a>
  <a href="https://t.me/skdev29">
    <img src="https://img.shields.io/badge/Telegram-Community-2CA5E0?style=for-the-badge&logo=telegram" alt="Telegram" />
  </a>
</p>

---

## ✨ What is Aniset?

**Aniset** is an Android widget pack built on top of [KWGT (Kustom Widget Maker)](https://play.google.com/store/apps/details?id=org.kustom.widget). It provides a curated collection of anime-inspired widgets that let you transform your home screen with stunning visuals from your favorite anime series.

This repository hosts the **asset backend** — JSON API files and media assets (wallpapers, ringtones) served via GitHub raw URLs. It powers the current **Aniset** app and will also serve as the content source for two upcoming apps:

| App | Description | Status |
|---|---|---|
| **Aniset** | Anime KWGT widget pack | ✅ Live on Play Store |
| **Aniset Pro** | Paid anime widget app with expanded presets & new designs | 🚧 Coming Soon |
| **Anify** | Free standalone anime wallpaper & ringtone app | 🚧 Coming Soon |

## 🚀 Key Features

- **🎨 Anime-Themed Widgets** — Beautifully designed KWGT presets inspired by popular anime
- **🖼️ 100+ Wallpapers** — High-quality 1080p anime wallpapers with optimized WebP thumbnails
- **🔔 Ringtones** — Anime notification & ringtone sounds (e.g. Pikachu Message tone)
- **🔄 Regular Updates** — New widgets, wallpapers, and content added frequently
- **📱 Wide Compatibility** — Works on smartphones and tablets running Android
- **⭐ Aniset Pro** — Upcoming paid widget app with expanded anime presets & new designs
- **📦 Anify** — Upcoming free standalone anime wallpaper & ringtone app

## 📂 Project Structure

```
aniset/
├── Wallpaper.json      # Main wallpaper catalog (100+ entries)
├── Anify.json           # Anify wallpaper catalog
├── Ringtones.json       # Ringtone catalog
├── Wallpapers/
│   ├── W/               # Full-resolution wallpapers (JPEG/PNG)
│   └── T/               # Optimized thumbnails (WebP)
├── anify/
│   └── ringtone/        # Ringtone audio files (MP3)
└── index.html           # Landing page
```

## 🔌 JSON API

The app consumes JSON files from this repo as a lightweight content API via GitHub raw URLs.

### Wallpaper Entry

```json
{
  "name": "1",
  "author": "Aniset",
  "url": "https://raw.githubusercontent.com/satyakiran29/aniset/main/Wallpapers/W/1%20(1).jpeg",
  "thumbnail": "https://raw.githubusercontent.com/satyakiran29/aniset/main/Wallpapers/T/1%20(1).webp",
  "dimensions": "1080p",
  "copyright": "Free"
}
```

### Ringtone Entry

```json
{
  "name": "Pikachu Message.mp3",
  "author": "Anify",
  "url": "https://satyakiran29.github.io/aniset/anify/ringtone/Pikachu%20Message.mp3",
  "duration": "0:1"
}
```

| Endpoint | Description |
|---|---|
| `Wallpaper.json` | Full wallpaper catalog with thumbnails |
| `Anify.json` | Anify-section wallpapers |
| `Ringtones.json` | Available ringtone sounds |

## 🛠️ Getting Started

### Prerequisites

- An Android device with [KWGT Kustom Widget Maker](https://play.google.com/store/apps/details?id=org.kustom.widget) installed
- [Aniset app](https://play.google.com/store/apps/details?id=com.skdev.aniset) from the Google Play Store

### Usage

1. **Install** KWGT and the Aniset app from the Play Store
2. **Long-press** on your home screen → Add Widget → KWGT
3. **Tap** the widget to open KWGT editor
4. **Browse** the Aniset preset tab and pick a widget
5. **Save** — enjoy your anime-themed home screen!

### For Developers

Clone the repo to explore or contribute assets:

```bash
git clone https://github.com/satyakiran29/aniset.git
```

#### Adding a New Wallpaper

1. Place the full-resolution image in `Wallpapers/W/`
2. Create an optimized WebP thumbnail in `Wallpapers/T/`
3. Add an entry to `Wallpaper.json` following the existing schema
4. Commit and push — the app will pick up the new content automatically

## 🗺️ Roadmap

- [x] Aniset KWGT widget pack — live on Play Store
- [x] Wallpaper catalog with 100+ anime wallpapers
- [x] Ringtone collection
- [ ] **Aniset Pro** — Paid widget app with expanded anime presets & new designs
- [ ] **Anify** — Free standalone anime wallpaper & ringtone app with favorites, categories & daily picks

## 📸 Screenshots

Check out the full screenshot gallery on the [Aniset website](https://aniset.vercel.app/Screenshot.html).

## 🤝 Contributing

Contributions are welcome! Whether it's new wallpapers, ringtones, or bug fixes:

1. **Fork** this repository
2. **Create** a feature branch (`git checkout -b feature/new-wallpapers`)
3. **Add** your assets following the project structure above
4. **Commit** your changes (`git commit -m "Add new wallpapers"`)
5. **Push** to the branch (`git push origin feature/new-wallpapers`)
6. **Open** a Pull Request

> **Note:** Please ensure all wallpapers are copyright-free or that you have the rights to distribute them.

## 💬 Support & Community

<blockquote>
  <strong>⚠️ Why is the Play Store price higher?</strong><br/>
  Due to refund abuse and Play Store taxes, the price on the Play Store has been increased. To avoid the Play Store tax, discounted pricing is available for direct purchases — contact <a href="https://t.me/skdev1">@skdev1 on Telegram</a> for details.
</blockquote>

| Channel | Link |
|---|---|
| 🌐 Website | [aniset.vercel.app](https://aniset.vercel.app/) |
| 💬 Telegram Group | [t.me/skdev29](https://t.me/skdev29) |
| 📩 Developer Contact | [t.me/skdev1](https://t.me/skdev1) |
| 🛒 Google Play | [Aniset on Play Store](https://play.google.com/store/apps/details?id=com.skdev.aniset) |

## 👤 Maintainer

[@satyakiran29](https://github.com/satyakiran29)

For special discounts or business inquiries, reach out on [Telegram](https://t.me/skdev1).

---

<p align="center">
  Made with ❤️ for the anime community
</p>
