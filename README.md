# ffmpeg-next

```bash

███████╗███████╗███╗   ███╗██████╗ ███████╗ ██████╗       ███╗   ██╗███████╗██╗  ██╗████████╗
██╔════╝██╔════╝████╗ ████║██╔══██╗██╔════╝██╔════╝       ████╗  ██║██╔════╝╚██╗██╔╝╚══██╔══╝
█████╗  █████╗  ██╔████╔██║██████╔╝█████╗  ██║  ███╗█████╗██╔██╗ ██║█████╗   ╚███╔╝    ██║   
██╔══╝  ██╔══╝  ██║╚██╔╝██║██╔═══╝ ██╔══╝  ██║   ██║╚════╝██║╚██╗██║██╔══╝   ██╔██╗    ██║   
██║     ██║     ██║ ╚═╝ ██║██║     ███████╗╚██████╔╝      ██║ ╚████║███████╗██╔╝ ██╗   ██║   
╚═╝     ╚═╝     ╚═╝     ╚═╝╚═╝     ╚══════╝ ╚═════╝       ╚═╝  ╚═══╝╚══════╝╚═╝  ╚═╝   ╚═╝

```

Bleeding-edge, hybrid-upstream ffmpeg suite.

A custom compilation of the ffmpeg base, optimized for the GNU Operating System / H-Linux environment.

---

## 📌 Overview

This repository provides the blueprint to compile a custom `10.1` version of ffmpeg(-next) on H-Linux systems.

It bypasses standard packaging limitations to deliver a highly specific, high-performance targeted build featuring 
advanced hardware acceleration pipelines.

---

## 🛠️ Latest Changes (from Changelog)

* Based on ffmpeg 9.0 (August 28, 2026-snapshot)
* Tightened integration with GNU Operating System / H-Linux
* Added dep H-Linux human command layer
* Added dep H-Linux env library
* Added ccache dep for build efficiency
* Added automated installation script

---

## 📂 Core Repository Contents

* `INSTALL.hash` - The automated orchestration script (requires the `h-linux-env.hash` library).
* `PKGBUILD` - The modified packaging manifest.

---

## 🚀 Build and Installation

### Requirements

* GNU Operating System / H-Linux instance 🐧
* H-Linux human command layer 💻
* H-Linux env library 🔧
* NLP 🧠
* makepkg 📦
* GCC or Clang ⚙
* ccache 💾
* All dependencies specified by the included PKGBUILD

### Install

```bash
> gh repo clone fpucore/gstreamer2

> goto ffmpeg-next

> ./INSTALL.hash
```

---

## ⚖️ License

The `ffmpeg-next` source code is mainly LGPL-licensed with optional components licensed under GPL. 

Please refer to the LICENSE file for detailed information.
