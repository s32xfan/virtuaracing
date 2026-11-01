# Third-Party Notices and Credits

This document covers third-party software, libraries, and algorithms utilized by the VR32X native runtime and pre-compiled release binaries.

---

## Runtime Libraries

### TinyCC / libtcc (LGPL 2.1)
- Used as the local C-to-native machine code compiler for the ROM-derived AOT execution cache.
- The pre-compiled Linux release bundles `libtcc.so` (version 0.9.28rc, based on the Blosc/minicc fork).
- The pre-compiled Windows release bundles `tcc.dll` (normalized to the system UCRT).
- TinyCC is licensed under the **GNU Lesser General Public License v2.1 (LGPL 2.1)**.
- Upstream project and source code: <https://bellard.org/tcc/>
- Full LGPL 2.1 text: <https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html>

### SDL2 (zlib License)
- The native runtime links dynamically against the host system's installed SDL2 library (`libSDL2.so` on Linux, system runtime on Windows).
- Upstream: <https://libsdl.org/>

---

## Graphics Algorithms & Visual Techniques

The native renderer incorporates independent, clean-room shader implementations of visual techniques originated by third parties:

- **MMPX Pixel-Art Magnification:**  
  Shader implementation inspired by the MMPX algorithm by Morgan McGuire and Mara Gagiu (*"MMPX Style-Preserving Pixel Art Magnification"*, 2021).  
  Reference & MIT License: <https://casual-effects.com/research/McGuire2021PixelArt/>

- **FXAA (Fast Approximate Anti-Aliasing):**  
  Implementation based on the FXAA algorithm by Timothy Lottes (NVIDIA Corporation).  
  Licensed under the 3-Clause BSD License: <https://developer.download.nvidia.com/assets/gamedev/files/sdk/11/FXAA_WhitePaper.pdf>

- **SMAA (Subpixel Morphological Anti-Aliasing):**  
  Original, lookup-table-free implementation inspired by the general morphological antialiasing technique by Jimenez et al. (2012).

- **GTAO (Ground Truth Ambient Occlusion):**  
  Original horizon-based ambient occlusion implementation based on the principles published by Jimenez et al. (Activision, 2016).

---

## Typography

- **DejaVu Sans Mono:**  
  Bitmap glyph coverage utilized by the configuration overlay is derived from the DejaVu Fonts family.  
  Licensed under the DejaVu Fonts License (Bitstream Vera derivative): <https://dejavu-fonts.github.io/License.html>

---

## Project License

All original runtime code and documentation for this project are released under the MIT License — see [`LICENSE`](LICENSE) and [`NOTICE`](NOTICE).
