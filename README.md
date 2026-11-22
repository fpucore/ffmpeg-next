# ffmpeg-next

```bash

███████╗███████╗███╗   ███╗██████╗ ███████╗ ██████╗       ███╗   ██╗███████╗██╗  ██╗████████╗
██╔════╝██╔════╝████╗ ████║██╔══██╗██╔════╝██╔════╝       ████╗  ██║██╔════╝╚██╗██╔╝╚══██╔══╝
█████╗  █████╗  ██╔████╔██║██████╔╝█████╗  ██║  ███╗█████╗██╔██╗ ██║█████╗   ╚███╔╝    ██║   
██╔══╝  ██╔══╝  ██║╚██╔╝██║██╔═══╝ ██╔══╝  ██║   ██║╚════╝██║╚██╗██║██╔══╝   ██╔██╗    ██║   
██║     ██║     ██║ ╚═╝ ██║██║     ███████╗╚██████╔╝      ██║ ╚████║███████╗██╔╝ ██╗   ██║   
╚═╝     ╚═╝     ╚═╝     ╚═╝╚═╝     ╚══════╝ ╚═════╝       ╚═╝  ╚═══╝╚══════╝╚═╝  ╚═╝   ╚═╝

+AV2
```

Bleeding-edge, hybrid-upstream **ffmpeg+AV2** suite.

A custom compilation of the ffmpeg base, optimized for the GNU Operating System / H-Linux environment.

Includes **LAME** codec dependency checker, and the **AV2** codec components.

---

## 📌 Overview

This repository provides the development blueprint to compile a custom `10.3.1` version of ffmpeg(-next) on GNU 
Operating System / H-Linux systems, including additional LAME codec checker and AV2 components.

It bypasses standard packaging limitations to deliver a highly specific, high-performance targeted build featuring 
advanced hardware acceleration pipelines.

---

## 🛠️ Latest Recent Changes (from Changelog)

* Based on ffmpeg 9.1 (November 2026-snapshot)
* Tightened integration with GNU Operating System / H-Linux
* Added dep H-Linux Human Command Layer
* Added dep H-Linux Environment Library
* Added ccache dep for compile efficiency
* Added automated installation script
* LAME codec dependency checker
* AV2 codec compile with smart adaption procedure

---

## 📂 Core Repository Contents

* `INSTALL.hash` - The advanced, automated hybrid-orchestration script (requires the `h-linux-env.hash` library).
* `PKGBUILD` - The modified packaging manifest.

---

## 🚀 Build and Installation

### Requirements

* GNU Operating System / H-Linux instance 🐧
* H-Linux Human Command Layer 💻
* H-Linux Environment Library 🔧
* NLP 🧠
* makepkg 📦
* GCC or Clang ⚙
* ccache 💾
* LAME (codec)
* All dependencies specified by the included PKGBUILD

### Install

```bash
> gh repo clone fpucore/ffmpeg-next

> goto ffmpeg-next

> $here/INSTALL.hash
```

---

## ⚖️ License

The `ffmpeg-next` source code is mainly LGPL-licensed with optional components licensed under GPL. 

Please refer to the LICENSE file for detailed information.

The `AV2` components are licensed under BSD 3-Clause Clear License The Clear BSD License.
