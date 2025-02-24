# Rust Browser Engine

Welcome to the **Rust Browser Engine**, an ambitious open-source project to build a fast, modern, and extensible web browser engine from scratch using Rust and the `iced` UI framework. The goal? To rival Chrome’s performance and features while targeting Windows, Mac, Linux, and Android.

## Project Overview

This browser engine aims to deliver a complete web browsing experience with:
- **Core Features**: Full HTML5, CSS3, and ES6+ support.
- **Performance**: GPU-accelerated rendering and caching for speed.
- **Extensibility**: A custom Extensions API for user add-ons.
- **Cross-Platform**: Native builds for desktop (Windows, Mac, Linux) and mobile (Android).

Built in Rust for safety and speed, with `iced` providing a lightweight, native UI, this project is a long-term effort to redefine browsing.

## Tech Stack

- **Language**: Rust
- **Key Crates**: `html5ever` (HTML parsing), `cssparser` (CSS), `skia-safe`/`wgpu` (rendering), `rusty_v8` (JS), `hyper`/`tokio` (networking), `iced` (UI), `sled` (cache), `rayon` (optimization).
- **Tools**: `cargo`, `cargo-ndk`, Git, Android NDK.

## Learning Plan Summary

To build this, I’m mastering:
1. **Rust**: Core language skills (ownership, async, etc.).
2. **Web Standards**: Deep dive into HTML5, CSS3, JS implementation.
3. **Graphics**: Rendering with `wgpu` and `skia-safe`.
4. **Networking**: HTTP via `hyper`.
5. **Internals**: Browser engine architecture.
6. **UI**: `iced` for native interfaces.
7. **Android**: NDK for mobile support.

Leveraging my HTML5, CSS3, and JS skills, I expect 6-12 months of learning. See [Learning_Plan.md](./Learning_Plan.md) for details.

## Build Steps Summary

The engine’s built in phases:
1. **Foundation**: Parser, renderer, CSS (3-6 months).
2. **Core Features**: Layout, JS, networking (6-12 months).
3. **UI & Polish**: Tabs, advanced rendering (12-18 months).
4. **Chrome-Killer**: Standards, cache, extensions, release (18-36+ months).

Total solo build time: 3-5+ years. Check [Build_Steps.md](./Build_Steps.md) for the full roadmap.

## Engine Parts

Key components include:
- HTML Parser, CSS Parser, DOM, Layout Engine, Rendering Engine.
- JS Runtime, Networking, Security, Event System.
- Cache and Extensions API for performance and flexibility.

## Getting Started

1. Clone the repo: `git clone https://github.com/<your-username>/rust-browser.git`
2. Install Rust: `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`
3. Add targets: `rustup target add x86_64-pc-windows-msvc x86_64-apple-darwin x86_64-unknown-linux-gnu aarch64-linux-android`
4. Build: `cargo build`

## Contributing

This is early days—contributions are welcome! Check the build steps or ping me with ideas. Focus areas: parsing, rendering, UI, or Android support.

## License

TBD (to be decided as the project matures).

## Links

- [Learning Plan](./Learning_Plan.md): Skills I’m tackling.
- [Build Steps](./Build_Steps.md): Roadmap to completion.
