# Vitaliy Alexeyev

Systems engineer — Rust, GPU/CUDA, ML infrastructure. Low-level and
performance-first, with 15+ years across hardware, firmware, and software. Based
in Kostanay, Kazakhstan; open to remote work or relocation.

I spent years close to the metal — repairing electronics, writing bare-metal
firmware, designing PCBs — and now build systems software in Rust: a from-scratch
ML inference stack and a GPU-rendered GUI framework, both without a Python runtime.

### Projects

**[syngui](https://github.com/vitamindb/syngui)** — a retained-mode GUI framework
in Rust (~112k lines). wgpu rendering, an own text stack (shaping, glyph atlas,
color emoji), a CSS-like styling language with cascade and animations, 70+ widgets
(terminal, code editor, charts, tables, video). Runs on desktop, Android, and
WebAssembly. MIT / Apache-2.0.

**synaptix** — a native Rust engine for running and training models: an alternative
to the Python ML stack, no PyTorch, no Python runtime. Custom CUDA kernels via NVRTC
with NVFP4 / MXFP8 quantization, checked bit-for-bit against reference
implementations. Runs LLMs, image and video diffusion, and speech models locally on
a single GPU. *(open-sourcing soon)*

**synthos** — a desktop AI workstation built on syngui and synaptix, and the code
editor I use daily: node-based pipelines, chat, speech-to-text, text-to-speech,
diarization, and local retrieval. *(soon)*

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
