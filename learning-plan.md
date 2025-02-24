# Learning Plan for Browser Engine Development

This outlines the skills and technologies I need to master to build a Chrome-killing browser engine in Rust with `iced` for Windows, Mac, Linux, and Android. My existing skills (HTML5, CSS3, JavaScript) are leveraged, and new areas are prioritized in an ordered sequence.

## Core Skills to Learn

| **Skill**             | **Why I Need It**                              | **What to Focus On**                              | **Resources**                       | **Estimated Time** |
|-----------------------|------------------------------------------------|--------------------------------------------------|-------------------------------------|--------------------|
| 1. Rust Mastery       | Core language for engine and UI               | Ownership, borrowing, async, unsafe Rust         | *The Rust Book*, *Rust by Example*, Servo GitHub | 1-3 months        |
| 2. Web Standards      | Implement HTML5, CSS3, JS parsing/rendering   | DOM structure, CSS rules, JS execution           | MDN Web Docs, WHATWG, W3C specs    | 1-2 months        |
| 3. Graphics Programming | Render web pages (text, images, WebGL)       | OpenGL/Vulkan via `wgpu`, 2D with `skia-safe`    | LearnOpenGL.com, `wgpu` docs, Skia | 2-4 months        |
| 4. Networking         | Fetch web resources (HTTP/HTTPS)              | HTTP protocols, `hyper`/`reqwest` in Rust        | HTTP RFC 9110, `tokio` docs        | 1-2 months        |
| 5. Browser Internals  | Understand engine architecture                | Parsing → DOM → Layout → Render pipeline         | Servo source, WebKit blogs         | 2-3 months        |
| 6. UI with `iced`     | Build native UI for browser shell             | `iced`’s Elm-like model, canvas rendering        | `iced` docs, GitHub examples       | 1-2 months        |
| 7. Android Development| Port to Android                               | NDK, `cargo-ndk`, touch events                  | Android NDK docs, Rust Android guides | 2-3 months       |

## Existing Skills and Their Role

| **Skill**     | **How It Helps**                              | **Relevance**                          |
|---------------|-----------------------------------------------|----------------------------------------|
| HTML5         | Understand what the parser needs to handle    | High - Direct overlap with engine input |
| CSS3          | Know styling rules to implement in CSS parser | High - Guides layout and rendering     |
| JavaScript    | Grasp JS behavior for runtime integration     | High - Informs `rusty_v8` usage        |
| Java          | Possible Android edge cases (JNI)             | Low - Rust covers most needs           |
| React         | Conceptual overlap with `iced`’s UI model     | Medium - Eases UI learning             |
| Next.js       | Minimal; JS knowledge helps                   | Very Low - Server-side irrelevant      |
| Bootstrap     | CSS3 knowledge applies, but not framework     | Very Low - No direct use               |
| Tailwind      | CSS3 knowledge applies, but not utility classes | Very Low - No direct use            |

## Learning Steps

### 1. Learn Rust Basics
- **Duration**: 1-2 months
- **Tasks**: Variables, functions, ownership/borrowing; build a CLI app (e.g., file reader).
- **Goal**: Comfort with Rust syntax and safety.

### 2. Deepen Web Standards Knowledge
- **Duration**: 1-2 months (parallel with Rust)
- **Tasks**: Study DOM, CSS rendering, JS event loop; sketch a mini HTML → DOM parser.
- **Goal**: Shift from user to implementer mindset.

### 3. Intro to Graphics with Rust
- **Duration**: 2-3 months
- **Tasks**: Learn `skia-safe` and `wgpu`; draw a square in `iced`.
- **Goal**: Render simple visuals.

### 4. Rust Advanced + Networking
- **Duration**: 2-3 months
- **Tasks**: Async with `tokio`, fetch web pages with `hyper`.
- **Goal**: Handle web requests in Rust.

### 5. Browser Internals
- **Duration**: 2-3 months (overlapping)
- **Tasks**: Study Servo, trace a page’s pipeline.
- **Goal**: Grasp engine flow.

### 6. UI with `iced`
- **Duration**: 1-2 months
- **Tasks**: Build a simple `iced` app (button + text).
- **Goal**: Native UI skills.

### 7. Android Prep
- **Duration**: 2-3 months (later)
- **Tasks**: Learn NDK, port an `iced` app to Android.
- **Goal**: Mobile readiness.

## Total Learning Time
- **Range**: 6-12 months, depending on pace and overlap.
