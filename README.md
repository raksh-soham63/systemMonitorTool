# 🖥️ System Monitor

A lightweight **C++ System Monitor** that provides real-time insights into your system’s CPU usage, memory utilization, and running processes.  
Designed with **modern C++** and a modular architecture, this tool demonstrates efficient process management and resource tracking — perfect for systems programming and performance monitoring.

![Preview Image](PreviewSS.jpg)

---

## 🚀 Features

- 📊 Real-time CPU & memory monitoring  
- ⚙️ Process list with PID, CPU%, and memory%  
- 🧩 Modular architecture using C++ classes  
- 🧱 Built with **CMake** for portability  
- 🐋 **Docker** support for easy containerized execution  
- 💡 Cross-platform (Linux / macOS)

---

## 🗂️ Project Structure

```
system-monitor/
├── src/
│   ├── main.cpp
│   ├── system_info.hpp / .cpp   # Collects CPU & memory statistics
│   ├── process.hpp / .cpp       # Handles process management
│   ├── utils.hpp / .cpp         # Utility helpers and formatting
├── CMakeLists.txt               # Build configuration
├── Makefile                     # Optional build script
├── Dockerfile                   # Container setup
└── README.md                    # Project documentation
```

---

## ⚙️ Build Instructions

### 🧰 Prerequisites

Ensure you have the following installed:

- **CMake** ≥ 3.10  
- **g++** or **clang++**  
- **Make** (optional)  
- **Docker** (optional)

---

### 🏗️ Build with CMake

```bash
mkdir build && cd build
cmake ..
make
./system-monitor
```

### 🧱 Build with Makefile (alternative)

```bash
make
./system-monitor
```

---

## 🐋 Run with Docker

To build and run inside a container:

```bash
docker build -t system-monitor .
docker run --rm -it system-monitor
```

---

## 🧠 How It Works

- `system_info.cpp` — Collects and parses CPU/memory data from `/proc` (Linux).  
- `process.cpp` — Enumerates active processes, calculating usage metrics.  
- `utils.cpp` — Provides helper functions for formatting and system queries.  
- `main.cpp` — Ties it all together for a live, readable output.

---

## 📊 Example Output

```
-------------------------------------
System Monitor
CPU Usage: 37%
Memory Usage: 58%
-------------------------------------
PID   Name          CPU%   MEM%
1023  firefox       14.2   9.8
2281  code          22.6   12.1
4321  terminal      2.3    0.9
-------------------------------------
```

---

## 👨‍💻 Author

**Soham Rakshit**  
🔗 [GitHub Soham Rakshit](https://github.com/raksh-soham63)

---

## 🏷️ Badges

![C++](https://img.shields.io/badge/language-C%2B%2B-blue.svg)
![CMake](https://img.shields.io/badge/build-CMake-lightgrey.svg)
![Docker](https://img.shields.io/badge/containerized-Docker-blue.svg)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)


