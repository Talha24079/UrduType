# UrduType — Urdu & Quranic Text Editor

A modern, cross-platform text editor specifically designed for **Urdu** and **Quranic text** with accurate **Nastaliq shaping**.

## ✨ Features


- **Advanced Text Shaping** — HarfBuzz-powered Nastaliq rendering  
- **Cross-Platform** — Works on Windows, Linux, and macOS  
- **PDF Export** — Preserve complex text shaping in exported documents  
- **Modern UI** — Qt 6-based intuitive interface  
- **Font Management** — Full support for Urdu-specific fonts  

## 🛠️ Built With


| Component | Purpose |
|------------|----------|
| **C++20** | Core programming language |
| **Qt 6** | Cross-platform GUI framework |
| **HarfBuzz** | Text shaping engine |
| **FreeType** | Font rendering library |
| **CMake** | Build and project management system |

## 📦 Installation

### Prerequisites

- **Qt 6.9.3** or later  
- **C++20** compatible compiler  
- **vcpkg** for dependency management  

### 🪟 Windows (Visual Studio 2022)

```powershell
# Clone and setup
git clone https://github.com/your-username/urdu-type.git
cd urdu-type

# Run setup script
scripts\setup_env.bat

# Build with CMake
cmake -B build -S .
cmake --build build --config Release
```

### 🐧 Linux / 🍎 macOS

```bash
# Clone and setup
git clone https://github.com/your-username/urdu-type.git
cd urdu-type

# Setup environment
chmod +x scripts/setup_env.sh
./scripts/setup_env.sh

# Build
cmake -B build -S .
cmake --build build --config Release
```

## 🚀 Usage

1. Launch **UrduType**  
2. Load or create a new document  
3. Type Urdu/Arabic text — shaping is applied automatically  
4. Use formatting tools for styling  
5. Export to **PDF** with preserved text layout  

## 🗂️ Project Structure

```
UrduType/
├── include/          # Header files
├── src/              # Source files
├── assets/fonts/     # Font resources
├── scripts/          # Build and setup scripts
└── tests/            # Unit tests
```

## 📄 License

Distributed under the **MIT License**.  
See [`LICENSE`](LICENSE) for more information.
