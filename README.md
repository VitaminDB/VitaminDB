# Vitaliy Alexeyev

Systems engineer — Rust, GPU/CUDA, ML infrastructure. Low-level and
performance-first, with 15+ years across hardware, firmware, and software. Based
in Kostanay, Kazakhstan; open to remote work or relocation.

I spent years close to the metal — repairing electronics, writing bare-metal
firmware, designing PCBs — and now build systems software in Rust: a from-scratch
ML inference stack and a GPU-rendered GUI framework, both without a Python runtime.

### Projects

**[synthos](https://github.com/VitaminDB/synthos)** — a local AI desktop studio
(~143k lines): an agentic chat that runs 27B–125B models from single-file bundles, a
block-based notes workspace (canvas, kanban, Gantt, mind maps, calendar), a node
editor for video / music / speech generation, a code editor and a local knowledge
base. Everything on-device, no Python. MIT / Apache-2.0.

**[synaptix](https://github.com/VitaminDB/synaptix)** — a native Rust engine for
running and training models (~232k lines, 1800+ tests): an alternative to the Python
ML stack, no PyTorch, no Python runtime. Hand-written CUDA kernels via NVRTC with
NVFP4 / MXFP8 quantization, checked bit-for-bit against reference implementations.
Gemma-4 26B at 210 tok/s decode, a 125B MoE with a 262k context on a 24 GB laptop
card. MIT / Apache-2.0.

**[syngui](https://github.com/VitaminDB/syngui)** — a retained-mode GUI framework in
Rust (~166k lines). wgpu rendering, an own text stack (shaping, glyph atlas, color
emoji), a CSS-like styling language with cascade and animations, 110+ widgets
(terminal, code editor, block document editor, charts, tables, video). Runs on
desktop, Android, and WebAssembly. MIT / Apache-2.0.

Earlier commercial work: a central-heating controller with a custom architecture and
GSM-OTA bootloader (in production for years), and a Qt/C++ SPI-flash recovery tool
used daily in an electronics-repair shop.

### Skills

Rust · C++ · Assembly (x86 / AVR / PIC) · CUDA (NVRTC runtime kernels, GEMM/GEMV,
fused kernels, NVFP4 / FP8 quantization, Nsight profiling) · wgpu / WGSL · embedded
(STM32, AVR, PIC; bare-metal, DMA, bootloaders) · Linux (Arch) · FFI · KiCad

### Approach

Self-taught across the stack. I verify claims instead of trusting them — I benchmark
and profile my own work and report the real numbers, including where it loses.

### Contact

Email — vitamindbnfkz@gmail.com

If any of this is useful to you, you can support the work via
[PayPal](https://paypal.me/vitamindbnfkz).
