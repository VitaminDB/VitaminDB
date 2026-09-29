# Vitaliy Alexeyev

Systems engineer — Rust, GPU/CUDA, ML inference, desktop software for Linux. Based in
Kostanay, Kazakhstan; open to remote work or relocation.

**Everything below is vibe-coded.** Since spring 2026 I write all of my projects with
[Claude Code](https://claude.com/claude-code): I decide what to build and how it fits
together, describe each task, and review, run and measure the result on my own hardware —
the model writes the code. That is how one person ends up with a CUDA inference engine, a
GUI framework, an AI studio and a Wayland desktop in half a year. The numbers in each README
are measured on my machine, not taken on the model's word.

### Projects

| | |
|---|---|
| **[synthos](https://github.com/VitaminDB/synthos)** | Local AI desktop studio: agentic chat, a notes workspace with boards and calendar, a node editor for image, video, music and speech generation, a code editor. Runs 27B–125B models on one NVIDIA GPU. No Python, no cloud. On the AUR as `synthos-bin`. |
| **[synaptix](https://github.com/VitaminDB/synaptix)** | The engine under synthos: LLM, diffusion, video, speech and music models on hand-written CUDA kernels compiled at runtime through NVRTC. NVFP4 / MXFP8 / SQ quantization, GGUF loads directly; kernels checked bit-for-bit against reference implementations, 1800+ tests. Gemma-4 26B decodes at 210 tok/s. No PyTorch. |
| **[syngui](https://github.com/VitaminDB/syngui)** | Retained-mode GUI framework for Rust: wgpu rendering, CSS-like stylesheets, reactive signals, 110+ widgets — terminal, code and block-document editors, charts, video. Desktop, Android and WebAssembly. Every app here is built on it. |
| **[syndesktop](https://github.com/VitaminDB/syndesktop)** | Wayland desktop environment: smithay compositor, shell with a macOS-style dock and panels, system settings, file manager, screenshot tool. |
| **[linux-legion](https://github.com/VitaminDB/linux-legion)** | Lenovo Vantage for Linux: power modes, CPU limits, fans, per-key Spectrum RGB, battery modes. No root, no kernel module. |
| **[ardor-mouse](https://github.com/VitaminDB/ardor-mouse)** | Linux configurator for the ARDOR GAMING Edge Air Ultra mouse — DPI, RGB, button remapping. Reverse-engineered protocol. |

### Background

Fifteen years close to the metal before this — repairing electronics, bare-metal firmware,
PCB design. Earlier commercial work: a central-heating controller with a GSM-OTA bootloader
(in production for years) and a Qt/C++ SPI-flash recovery tool used daily in a repair shop.

Rust · CUDA (NVRTC, GEMM/GEMV, fused kernels, FP4/FP8 quantization, Nsight) · C++ ·
wgpu / WGSL · embedded (STM32, AVR, PIC) · Arch Linux · KiCad

### Approach

I verify claims instead of trusting them — mine and the model's. Every project is
benchmarked and profiled on real hardware, and the READMEs report where it loses too.

### Contact

[alexeyev.dev](https://alexeyev.dev/) · [X / Twitter](https://x.com/alexeyev_vitaly) · vitamindbnfkz@gmail.com ·
support the work via [PayPal](https://paypal.me/vitamindbnfkz)
