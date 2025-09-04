# 🎭 Drama Queen

**Drama Queen** is a multi-platform drama staging and directing application.  
It helps stage everything — from lighting, character placement, and script timing to sound design — all inside a 3D environment.

- Import your own 3D stage.
- Add cast members and props.
- Place and animate lights, sounds, and actions on a timeline.
- Export everything as a `.dq` file (`.dramaqueen`).
- Share or view projects online through the Drama Queen Portal.

This is the **first public edition (v0.x)**. Expect bugs, missing features, and plenty of iteration. Contributions are welcome!

---

## ✨ Features (First Edition)

- Cross-platform: **Windows, macOS, Linux**
- Import stage files (`.obj`, `.fbx`, `.glb`)
- Place characters and props in 3D
- Timeline editor (basic play/pause)
- Add and configure lights (position, color, direction, intensity)
- Add and configure sounds (volume, timing)
- Export to `.dq` file format

---

## 🚧 Roadmap

- [ ] Script editor (attach lines to characters + timeline)
- [ ] Cue system (trigger lights/sounds at specific times)
- [ ] Online viewer portal (basic playback mode)
- [ ] Ulla script support (customize UI, buttons, layouts)
- [ ] C++ scripting API (extend functionality)

Check the [project board](./docs/roadmap.md) for more details.

---

## 🛠 Building From Source

Drama Queen is written in **C++** on top of the custom Luna/Ulla engine.

### Requirements
- CMake ≥ 3.22
- C++20-compatible compiler (MSVC, Clang, or GCC)
- Dependencies (installed automatically with CMake FetchContent):
    - [SDL2](https://libsdl.org/)
    - [glm](https://github.com/g-truc/glm)
    - [assimp](https://github.com/assimp/assimp)

### Build
```bash
git clone https://github.com/your-org/dramaqueen.git
cd dramaqueen
mkdir build && cd build
cmake ..
cmake --build .
