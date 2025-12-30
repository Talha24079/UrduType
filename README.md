# UrduType — Urdu & Quranic Text Editor

A modern, cross-platform text editor specifically designed for **Urdu** and **Quranic text** with accurate **Nastaliq shaping**.

## ✨ Features

- **Advanced Text Shaping** — Custom C++ engine powered by HarfBuzz
- **Cross-Platform** — Pixel-perfect UI on Windows, Linux, and macOS via Avalonia
- **Hybrid Architecture** — High-performance C++ backend with a modern C# frontend
- **PDF Export** — Vector-based export with preserved ligatures
- **Modern UI** — Fluent-inspired interface with dark mode support

## 🛠️ Built With

| Component | Purpose |
|------------|----------|
| **C# / .NET 8** | UI Logic and Application Layer |
| **Avalonia UI** | Cross-platform XAML-based GUI |
| **C++20** | Core Text Processing Engine (Shared Library) |
| **HarfBuzz** | Text shaping (Backend) |
| **FreeType** | Font rendering (Backend) |

## 📦 Installation

### Prerequisites

- **.NET 8 SDK**
- **C++20** compatible compiler
- **CMake** (for building the C++ core)

### 🪟 Windows / 🐧 Linux / 🍎 macOS

```bash
# Clone the repository
git clone [https://github.com/your-username/urdu-type.git](https://github.com/your-username/urdu-type.git)
cd urdu-type

# 1. Build the C++ Core (The Engine)
cd core
cmake -B build -S . -DCMAKE_BUILD_TYPE=Release
cmake --build build
cd ..

# 2. Run the UI (The Frontend)
# The csproj is configured to load the compiled C++ library
dotnet run --project src/UrduType.UI/UrduType.UI.csproj
