# Vitaliy Alexeyev

Systems engineer — Rust, GPU/CUDA, ML inference, Linux desktop and phones. Based in Kostanay, Kazakhstan;
open to remote work or relocation.

[alexeyev.dev](https://alexeyev.dev/) · [LinkedIn](https://www.linkedin.com/in/vitaly-alexeyev-08546b21b/) ·
[X / Twitter](https://x.com/alexeyev_vitaly) · vitamindbnfkz@gmail.com

**Everything below is vibe-coded.** Since spring 2026 I write all of my projects with
[Claude Code](https://claude.com/claude-code): I decide what to build and how it fits together, describe each
task, and review, run and measure the result on my own hardware — the model writes the code. The numbers in each
README are measured on my machine, not taken on the model's word.

### My own stack

| | |
|---|---|
| **[synaptix](https://github.com/VitaminDB/synaptix)** | Neural-network engine without Python or PyTorch: hand-written CUDA kernels compiled at runtime through NVRTC, NVFP4 / MXFP8 on Blackwell, GGUF loads directly. A 125B MoE model runs on a 24 GB laptop GPU; in NVFP4 it is 1.43× faster than torch.compile + fp8 on the same card. 2,400+ tests, bit-exact against PyTorch row by row. |
| **[syngui](https://github.com/VitaminDB/syngui)** | Retained-mode GUI framework for Rust: wgpu rendering, a real CSS cascade with its own LSP, SolidJS-style signals, 110+ widgets — terminal, code and block-document editors, charts, video. Desktop, Android and WebAssembly. Every app here is built on it. |
| **[synshell](https://github.com/VitaminDB/synshell)** | Wayland desktop environment: a compositor on a smithay fork, shell with a 3D dock and panels, System Settings, a system AI daemon, a phone ↔ PC link with an MCP server, and dozens of apps. The same shell runs on Android phones. |
| **[synthos](https://github.com/VitaminDB/synthos)** | Local AI studio on synaptix: agentic chat, notes with boards and calendar, a node editor for image, video, music and speech generation. No cloud. AUR: `synthos-bin`. |

### Utilities (MIT, AUR)

| | |
|---|---|
| **[linux-legion](https://github.com/VitaminDB/linux-legion)** | Lenovo Vantage for Linux: power modes, CPU limits, fans, per-key Spectrum RGB, battery modes. 14 languages. No root, no kernel module. |
| **[ardor-mouse](https://github.com/VitaminDB/ardor-mouse)** | Configurator for ARDOR GAMING mice — Edge Air Ultra and Rukh so far, more to come: DPI, RGB, buttons, sensor, a live mouse in the app. Reverse-engineered protocol. |

### Background

Fifteen years close to the metal before this — repairing electronics, bare-metal firmware, PCB design.
In production since 2019: a central-heating controller with my own firmware, bootloader and GSM OTA updates;
STM32 firmware rewritten in Rust (Embassy); a heat and water metering system with a GUI on syngui.

Rust · CUDA (NVRTC, GEMM/GEMV, fused kernels, FP4/FP8 quantization, Nsight) · C++ · wgpu / WGSL · Wayland ·
Android GKI · embedded (STM32, AVR, PIC) · Arch Linux · KiCad

### Approach

I verify claims instead of trusting them — mine and the model's. Every project is benchmarked and profiled on
real hardware, and the READMEs report where it loses too.

Support the work via [PayPal](https://paypal.me/vitamindbnfkz).
