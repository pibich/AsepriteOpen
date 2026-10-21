# Aseprite (Custom Build)

This repository contains a personal build of [Aseprite](https://www.aseprite.org/) compiled from the official source release.

- **Version**: `v1.3.18.6`
- **Target OS**: Windows 11 (x64)
- **Backend**: Skia (`aseprite-m124` branch)
- **Compiler**: MSVC (Visual Studio Build Tools) + CMake & Ninja

---

## 🚀 Getting Started

To run the application:
1. Open the [`bin/`](./bin) directory.
2. Launch `aseprite.exe`.

> **Note**: Ensure the `data/` folder and `icudtl.dat` remain in the same directory as `aseprite.exe`.

---

## 🛠️ Build Summary

Built using the following configuration:
```bash
cmake -DCMAKE_BUILD_TYPE=RelWithDebInfo \
      -DLAF_BACKEND=skia \
      -DSKIA_DIR=C:\deps\skia \
      -DSKIA_LIBRARY_DIR=C:\deps\skia\out\Release-x64 \
      -DSKIA_LIBRARY=C:\deps\skia\out\Release-x64\skia.lib \
      -G Ninja ..
ninja aseprite
```

---

## 📜 Credits & Acknowledgments

This project is built directly from the open-source codebase of **Aseprite**. All credit goes to the original authors, maintainers, and contributors:

- **Original Repository**: [github.com/aseprite/aseprite](https://github.com/aseprite/aseprite)
- **Official Website**: [aseprite.org](https://www.aseprite.org/)
- **Authors**: David Capello and Igara Studio S.A. ([Authors List](https://github.com/aseprite/aseprite/blob/main/AUTHORS.md))
- **Skia Fork for Aseprite**: [github.com/aseprite/skia](https://github.com/aseprite/skia)

---

## ⚖️ License & Disclaimer

- **Aseprite** is a registered trademark of **Igara Studio S.A.**
- The source code of Aseprite is distributed under the [Aseprite EULA](https://github.com/aseprite/aseprite/blob/main/EULA.txt).
- This repository is intended for personal/educational use in accordance with Aseprite's End User License Agreement. If you find Aseprite useful, please support the creators by purchasing an official license at [aseprite.org](https://www.aseprite.org/) or on [Steam](https://store.steampowered.com/app/431730/Aseprite/).
