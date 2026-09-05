
V1 Visit here: https://partakithware.github.io/OxPy/

This Version with added support: 

Browser-native Web Desktop Environment (WDE) for Python, C, and WebAssembly development.

Overview

Ox-Py WDE is an experimental client-side operating environment implemented entirely in the browser using WebAssembly-based runtimes and persistent virtual filesystem layers.

The environment provides:

Multi-window desktop shell
POSIX-inspired terminal environment
Persistent filesystem via IDBFS
Python runtime through Pyodide
C compilation through TinyCC (TCC) compiled to WebAssembly
WebAssembly tooling and execution support
Integrated development utilities and file management

Ox-Py operates without a mandatory backend server and stores workspace data locally within the browser.

Architecture
Browser Runtime
├── Ox-Py Desktop Shell
│   ├── Window Manager
│   ├── Taskbar / Start Menu
│   ├── Context Menu System
│   └── Application Runtime
│
├── Runtime Layer
│   ├── Pyodide (Python 3)
│   ├── TinyCC (TCC → Wasm)
│   ├── WASI Runtime
│   └── WABT Toolkit
│
├── Virtual Filesystem
│   ├── IDBFS Persistence
│   ├── User Workspace Mounts
│   └── Local Account Storage
│
└── Integrated Applications
    ├── Terminal
    ├── File Explorer
    ├── Text Editor
    ├── Graphics Window
    └── Ox-Browser

The platform is intended for:

WebAssembly experimentation
Browser runtime research
Client-side systems experimentation
Educational runtime development
Portable development environment research
