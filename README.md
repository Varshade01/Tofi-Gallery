# Tofi-Gallery
small product flow: list of images → detailed page with common element transition, caching, page splitting; demonstrates real user-flows.

A modern Android app + UI library built with **Kotlin** and **Jetpack Compose**.  
It showcases a **photo gallery** powered by the Unsplash API, including offline caching, smooth transitions, and reusable UI components.  

This project is split into **multi-modules** (`app`, `ui-core`, `data`) and demonstrates best practices in modern Android development: **Clean Architecture, MVVM/MVI, Paging 3, Room, Compose UI**, and **CI/CD publishing of AAR libraries**.  

---

## ✨ Features

- 🚀 **Photo Grid** with infinite scroll (Paging 3)  
- 🖼 **Detail screen** with shared element transition  
- 📡 **Real API integration** (Unsplash)  
- 💾 **Offline support** with Room cache  
- 🎨 **Reusable UI components** (e.g., `PrimaryButton`) published as AAR  
- ⚡ **Optimized recomposition** and smooth UI performance  
- ☁️ **CI/CD** with GitHub Actions + GitHub Packages publishing  
- 📱 Built entirely with **Jetpack Compose + Material3**  

---

## 📂 Project Structure
├── app/ # Application module (navigation, screens, DI)
├── data/ # Networking + Room + Repository layer
├── ui-core/ # Reusable UI components (published as AAR)
└── docs/ # GIFs, videos, and documentation


---

## 🛠 Tech Stack

- **Language**: Kotlin, Coroutines, Flow  
- **UI**: Jetpack Compose, Material3, Coil  
- **Architecture**: MVVM / MVI, Clean Architecture principles  
- **Networking**: Retrofit, Moshi  
- **Database**: Room, Paging 3, RemoteMediator  
- **Dependency Injection**: Hilt  
- **Testing**: JUnit, Compose UI tests  
- **CI/CD**: GitHub Actions (Build, Test, Publish)  

---

## 📸 Demo

### Gallery Screen
![Gallery Grid](docs/gallery_grid.gif)

### Detail Screen
![Detail Transition](docs/detail_transition.gif)

---

## 🔌 Setup

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/Tofi-Gallery.git
2. Open in Android Studio (Giraffe+)
3. Add your Unsplash API key in local.properties UNSPLASH_ACCESS_KEY=your_key_here
4. Run the app 🚀

📦 Using ui-core library
You can consume the UI components library separately:
dependencies {
    implementation("com.github.yourusername.galleryx:ui-core:1.0.0")
}
Example:
PrimaryButton(
    text = "Click me",
    onClick = { /* TODO */ }
)

⚙️ CI/CD

Build & Test on every PR

Publish ui-core AAR on GitHub Packages when a new release tag is pushed (vX.Y.Z)

📈 Roadmap

 Add search functionality

 Add dark/light theme toggle

 Add user profile screen

 Improve animations with MotionLayout / Compose Animations

👨‍💻 Author

Ostap Kresan

📧 ostapkresan@gmail.com

💼 Android Developer | Kotlin, Jetpack Compose

📄 License
MIT License
Copyright (c) 2025 Ostap
