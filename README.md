# 🎵 Lane — modern music streaming app

> A full-stack music streaming application built with modern Android technologies and a robust backend infrastructure. Supports playback and previewing from **Spotify** and **SoundCloud**.

---

## 📱 Android Client

The Android app is developed with a focus on **clean architecture**, **MVVM**, and **high performance UI/UX**.

### ✅ Tech Stack

* **Jetpack Compose** — fully declarative UI layer with custom layouts, animations, and gesture handling.
* **ExoPlayer** — seamless audio streaming with waveform rendering, speed controls, and lyrics progress synchronization.
* **Pager** — vertical paging between tracks, optimized for low memory usage and smooth gesture experience.
* **Hilt** — dependency injection across ViewModels, Repositories, and UseCases.
* **Kotlin Coroutines + Flows** — fully asynchronous, reactive data layer with fine-grained control over playback, downloads, and UI events.
* **Retrofit + OkHttp** — efficient network stack with custom interceptors, body logging, and support for progressive stream loading.
* **kotlinx.serialization** and **Gson** — hybrid JSON parsing depending on data structure source.
* **Firebase Services** — used for analytics, crash reporting, and remote config.

### 📊 Architecture

* Modular clean architecture: `ui`, `domain`, `data`, `core`
* Reactive playback flow with custom `LyricsView`, progress-aware sliders, and dynamic content visibility.
* Efficient media preloading: Spotify tracks are preloaded entirely, SoundCloud streams are loaded in batches on scroll.

---

## 🧰 Backend Server

The backend is built in **Ktor**, containerized and optimized for high-performance media delivery and authentication.

### ✅ Tech Stack

* **Ktor** — lightweight asynchronous framework with coroutine-first routing and pipeline handling.
* **Koin** — dependency injection for services and repositories.
* **MongoDB** — document-based database for scalable music and user metadata storage.
* **AWS S3** — used for secure media hosting and preview storage.
* **Micrometer** — exposes Prometheus-compatible metrics for monitoring, rate limiting, and performance optimization.
* **Retrofit + OkHttp** — server-to-server calls to external APIs (Spotify, SoundCloud) with retry, caching, and header injection.

### 📉 Features

* Highly optimized SoundCloud and Spotify API integrations with fallback, stream caching, and metadata normalization.
* OAuth2 login with **Telegram** and **Google**.
* **JWT-based authentication** for mobile clients.
* **Rate limiting**, request caching, and concurrency management.
* Streaming endpoints support resumable download and partial content headers.

---

## 📸 Screenshots



![Frame 225](https://github.com/user-attachments/assets/b2041e1b-4994-49f8-a1ab-9978c6a80f0b)




---

## 🎓 Author

Created by **Nazar Sladkovskyi** — Android Developer, reverse engineer

---

## 🛜 Download

https://sklane.com

---

## 🚀 Status

> Project is in active development. Version 2.0 will include collaborative playlists, AI-powered recommendations, and offline sync.
