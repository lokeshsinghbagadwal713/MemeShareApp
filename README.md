# 📱 MemeShareApp

![Kotlin](https://img.shields.io/badge/Kotlin-1.9-blue?logo=kotlin)
![Android](https://img.shields.io/badge/Android-13-green?logo=android)
![License](https://img.shields.io/badge/License-MIT-yellow)

MemeShareApp is a fun Android application that fetches random memes from the internet and lets users share them with friends.
Built with **Kotlin**, **Volley** for networking, and **Glide** for smooth image loading.

---

## ✨ Features

* 🔄 Fetch random memes from [Meme API](https://meme-api.com/gimme)
* 🖼️ Glide image loading + caching
* 📤 Share via any app (WhatsApp, Instagram, Telegram, etc.)
* ⏭️ “Next Meme” button for quick refresh
* ⚡ Efficient **Singleton** `RequestQueue` with Volley

---

## 🛠️ Tech Stack

* **Language**: Kotlin
* **UI**: XML (ConstraintLayout)
* **Networking**: Volley
* **Image Loading**: Glide
* **Design Pattern**: Singleton

---

## 📸 Demo

Add screenshots or a short GIF demo here:

![Home](screenshots/home.png)
![Share](screenshots/share.png)

> Put your images in a `screenshots/` folder at the repo root.

---

## 📂 Project Structure

```
app/src/main/java/com/example/memeshareapp/
│
├── MainActivity.kt        # Main screen, loads & displays memes
├── MySingleton.kt         # Singleton for Volley RequestQueue
│
app/src/main/res/layout/
├── activity_main.xml      # Main UI layout
```

---

## ▶️ Getting Started

### 1) Prerequisites

* Android Studio (latest)
* Android SDK 33+
* Kotlin 1.9+

### 2) Clone the Repo

```bash
git clone https://github.com/yourusername/MemeShareApp.git
cd MemeShareApp
```

### 3) Build & Run

* Open in **Android Studio**
* Sync Gradle
* Connect a device / launch emulator
* Run the app 🚀

---

## 📦 Dependencies (app-level `build.gradle`)

```gradle
// Volley for networking
implementation 'com.android.volley:volley:1.2.1'

// Glide for image loading
implementation 'com.github.bumptech.glide:glide:4.15.1'
annotationProcessor 'com.github.bumptech.glide:compiler:4.15.1'
```

---

## 🏗️ Architecture

* **Activity** → Handles UI & user actions
* **Singleton (MySingleton)** → Manages a single Volley `RequestQueue`
* **Volley** → API requests
* **Glide** → Loads/caches images

---

## 🚀 Future Work

* [ ] Offline caching of memes
* [ ] Dark mode
* [ ] Save to gallery
* [ ] Favorites list
* [ ] Swipe gesture for next meme

---

## 🤝 Contributing

1. Fork the project
2. Create your feature branch: `git checkout -b feature/AmazingFeature`
3. Commit: `git commit -m "Add AmazingFeature"`
4. Push: `git push origin feature/AmazingFeature`
5. Open a Pull Request

---

## 🙌 Acknowledgements

* [Meme API](https://meme-api.com/gimme) for meme data
* [Volley](https://developer.android.com/training/volley)
* [Glide](https://github.com/bumptech/glide)

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for details.
