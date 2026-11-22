# Third-Party Notices

This application (see [LICENSE](LICENSE)) bundles the open-source components
listed below. Each remains under its own license; this application's own
LICENSE covers only the code V.Trinz wrote and does not limit the rights
these licenses give you.

The full license texts ship in the **`licenses`** folder next to this file
(and next to the program). The developer-facing reasoning behind each
obligation is in `internal_docs/LICENSES.md` in the source repository; it is
not shipped, but nothing an end user needs is missing from this file.

The versions below are those of the current build. Tag reading and writing is
this application's own code (no third-party tag library is bundled).

---

## Components under the GNU Lesser General Public License (LGPL)

These are shipped as separate, unmodified library files that the program
loads at run time. You may replace them with modified or other compatible
versions and use the program with those, and reverse-engineer the program to
the extent needed to debug such modifications (see the program's LICENSE,
section 4).

### Qt 6.11.2, PySide6 6.11.2, shiboken6 6.11.2 - LGPL-3.0

Copyright (C) The Qt Company Ltd. and other contributors.
https://www.qt.io/

- Files: `qt6*.dll`, `pyside6.abi3.dll`, `shiboken6.abi3.dll`, the `PySide6`
  and `shiboken6` folders (Python bindings, Qt plugins).
- License texts: `licenses/LGPL-3.0.txt`, which supplements
  `licenses/GPL-3.0.txt`.
- Source code: Qt - https://download.qt.io/official_releases/qt/6.11/6.11.2/ ;
  PySide6/shiboken6 - https://code.qt.io/cgit/pyside/pyside-setup.git
  (tag v6.11.2), also https://download.qt.io/official_releases/QtForPython/
- Qt itself contains third-party code (image format, font and text
  libraries among others), listed with their licenses at
  https://doc.qt.io/qt-6/licenses-used-in-qt.html

### libsndfile 1.2.2, with mpg123 and LAME - LGPL-2.1

libsndfile Copyright (C) Erik de Castro Lopo and contributors.
mpg123 Copyright (C) Michael Hipp and others (LGPL-2.1).
LAME 3.100 Copyright (C) Mike Cheng, Mark Taylor and the LAME project
(LGPL, version 2 or later).

- File: `_soundfile_data/libsndfile_x64.dll` (one library; FLAC, Ogg, Vorbis
  and Opus are built into it too - see the BSD section below - and Apple's
  ALAC codec, see the Apache-2.0 row there).
- License text: `licenses/LGPL-2.1.txt`.
- Source code: libsndfile - https://github.com/libsndfile/libsndfile/releases/tag/1.2.2 ;
  how this library file is built, with the codec versions it uses -
  https://github.com/bastibe/libsndfile-binaries ; LAME 3.100 -
  https://sourceforge.net/projects/lame/files/lame/3.100/ ; mpg123 -
  https://www.mpg123.de/download.shtml

### python-soxr 1.1.0 with libsoxr - LGPL-2.1

Python-SoXR Copyright (c) 2021 Myungchul Keum.
SoX Resampler Library Copyright (c) 2007-18 robs@users.sourceforge.net.

- File: `soxr/soxr_ext.pyd` (libsoxr is built into it).
- License texts: `licenses/LGPL-2.1.txt`, `licenses/python-soxr-LICENSE.txt`,
  `licenses/libsoxr-LICENSE.txt`; the PFFFT code inside it is under its own
  BSD-style license, `licenses/PFFFT-LICENSE.txt`.
- Source code (libsoxr included): https://github.com/dofuuz/python-soxr/releases/tag/v1.1.0

---

## Components under permissive licenses

These require that their copyright and license notices travel with the
program, which this file and the `licenses` folder do.

| Component | License | License text |
|---|---|---|
| WavPack 5.8.0 (`wavpack_lib/wavpackdll.dll`), Copyright (c) 1998-2024 David Bryant | BSD | `wavpack_lib/NOTICE.txt` |
| PortAudio V19.7.0 (`_sounddevice_data/portaudio-binaries/`), Copyright (c) 1999-2006 Ross Bencina and Phil Burk | MIT | `licenses/PortAudio-LICENSE.txt` |
| sounddevice 0.5.6, Copyright (c) 2015-2025 Matthias Geier | MIT | `licenses/sounddevice-LICENSE.txt` |
| soundfile 0.14.0, Copyright (c) 2013 Bastian Bechtold | BSD-3-Clause | `licenses/soundfile-LICENSE.txt` |
| FLAC 1.4.3, libogg, libvorbis, Opus 1.5.2 (inside `libsndfile_x64.dll`), Copyright Xiph.Org Foundation and contributors | BSD-3-Clause | https://xiph.org/licenses/bsd/ |
| Apple Lossless (ALAC) codec (inside `libsndfile_x64.dll`; libsndfile's `src/ALAC`), Copyright (c) 2011 Apple Inc. | Apache-2.0 | `licenses/Apache-2.0.txt` |
| NumPy 2.5.2, with the libraries it bundles (OpenBLAS, LAPACK, pocketfft, ...) | BSD-3-Clause and others | `licenses/NumPy-LICENSE.txt` |
| cffi 2.1.1 (`_cffi_backend.pyd`) | MIT-0 | `licenses/cffi-LICENSE.txt` |
| typing_extensions 4.16.0 | PSF-2.0 | `licenses/typing_extensions-LICENSE.txt` |
| Python 3.14.6 (`python314.dll`, standard library) | PSF-2.0 | `licenses/Python-LICENSE.txt` |
| OpenSSL 3.5.7 (`libcrypto-3.dll`, `libssl-3.dll`) | Apache-2.0 | `licenses/Apache-2.0.txt` |
| libffi (`libffi-8.dll`), expat, zlib, libmpdec, Zstandard - bundled with Python | MIT / zlib / BSD | `licenses/Python-incorporated-software.txt` |
| bzip2 1.0.8 (`_bz2.pyd`) | bzip2 license (BSD-style) | `licenses/bzip2-LICENSE.txt` |
| xz / liblzma (`_lzma.pyd`) | 0BSD | `licenses/xz-liblzma-LICENSE.txt` |
| Zstandard library (`_zstd.pyd`) | BSD-3-Clause | `licenses/zstd-LICENSE.txt` |
| SQLite 3.50.4 (`sqlite3.dll`) | Public domain | - |
| Microsoft Visual C++ runtime (`msvcp140*.dll`, `vcruntime140*.dll`) | Microsoft redistributable files | distributed under the Visual Studio redistribution terms |

### SciPy-derived signal-processing code - BSD-3-Clause

Copyright (c) 2001-2002 Enthought, Inc. 2003, SciPy Developers.
All rights reserved.
https://scipy.org

This app does not ship SciPy itself. Its `audio_tools_sp` module and the
"scipy replacements" in its compiled `audio_tools_cy_kernels` module contain
code ported from SciPy 1.18.1 (filter design, filtering, resampling,
spectral analysis, peak finding and the 1-D image filters). Redistribution
and use in source and binary forms, with or without modification, are
permitted under the 3-clause BSD license: the above copyright notice, this
list of conditions and the following disclaimer must be retained; neither
the name of the copyright holder nor the names of its contributors may be
used to endorse or promote products derived from this software without
specific prior written permission. THE SOFTWARE IS PROVIDED "AS IS",
WITHOUT WARRANTY OF ANY KIND. Full text:
https://github.com/scipy/scipy/blob/main/LICENSE.txt

The polyphase resampler (`upfirdn`) in that code derives from the "upfirdn"
library, Copyright (c) 2009, Motorola, Inc, used by SciPy with permission
under the same BSD terms; Motorola's name may not be used to endorse or
promote products derived from this software without specific prior written
permission.

### De-limiter model weights - MIT (Audio Restoration Toolbox only)

Copyright (c) 2023 jeonchangbin49 (Chang-Bin Jeon).
https://github.com/jeonchangbin49/De-limiter - C. Jeon and K. Lee, "Music
De-limiter Networks via Sample-wise Gain Inversion", WASPAA 2023.

The experimental AI de-limiter of the Disc Remaster tab runs these published
weights (converted to a numpy file, values unchanged). They ship only with
the full version, in `ai_models/delimiter/`, together with their MIT license
text (`LICENSE.txt`) and a README stating their source. SonicScope does
not contain them.

### ASIO - Steinberg ASIO SDK (Audio Restoration Toolbox only)

ASIO is a trademark and software of Steinberg Media Technologies GmbH.

The full version's ASIO output and input use code from the Steinberg ASIO
SDK, built into `_sounddevice_data/portaudio-binaries/libportaudio64bit-asio.dll`
and `native/asio_dsd_shim/build/asio_dsd_shim.dll`. SonicScope does not
contain them.

### Compiler runtime

The program is compiled with Nuitka. The Nuitka runtime code built into it
is covered by the Nuitka Runtime Library Exception, which allows programs
under any license; it places no conditions on this program.

---

## Linux build (tar.gz, .deb, AppImage)

The Linux packages contain the same components under the same licenses,
with the differences below. The file names given above are those of the
Windows build; on Linux the libraries are `.so` files of the same name
(`libQt6*.so.6`, `libpyside6.abi3.so.*`, `libshiboken6.abi3.so.*`,
`_soundfile_data/libsndfile_x86_64.so`, `soxr/soxr_ext.so`,
`libpython3.14.so.1.0`, ...).

| Component | Linux build | License text |
|---|---|---|
| Qt, PySide6, shiboken6 | 6.12.0, LGPL-3.0 - source: https://download.qt.io/official_releases/qt/6.12/6.12.0/ and https://code.qt.io/cgit/pyside/pyside-setup.git (tag v6.12.0) | `licenses/LGPL-3.0.txt`, `licenses/GPL-3.0.txt` |
| ICU 73 (`libicudata.so.73`, `libicui18n.so.73`, `libicuuc.so.73`), shipped with Qt, Copyright (c) Unicode, Inc. and others | Unicode License (with the third-party notices of ICU's dictionaries and data) | `licenses/ICU-LICENSE.txt` |
| NumPy | 2.5.4, with OpenBLAS (`libscipy_openblas64_*.so`) and the GCC runtime libraries `libgfortran` (GPL-3.0 with the GCC Runtime Library Exception) and `libquadmath` (LGPL-2.1-or-later, a separate, replaceable `.so`; source: https://gcc.gnu.org/git/?p=gcc.git;a=tree;f=libquadmath) | `licenses/NumPy-Linux-LICENSE.txt`, `licenses/LGPL-2.1.txt` |
| Python | 3.14.4 (`libpython3.14.so.1.0`, standard library), from Ubuntu's `libpython3.14` | `licenses/Python-LICENSE.txt` |
| OpenSSL | 3.5.5 (`libssl.so.3`, `libcrypto.so.3`) | `licenses/Apache-2.0.txt` |
| Ubuntu system libraries: libuuid (util-linux), expat, libffi, bzip2, xz/liblzma, Zstandard, SQLite 3.46.1 (`libuuid.so.1`, `libexpat.so.1`, `libffi.so.8`, `libbz2.so.1.0`, `liblzma.so.5`, `libzstd.so.1`, `libsqlite3.so.0`) | BSD-3-Clause / MIT / bzip2 license / 0BSD / BSD-3-Clause / public domain | `licenses/Linux-system-libraries.txt` (each package's copyright file) |
| PortAudio | not shipped - sounddevice uses the system's own PortAudio library | - |

The Microsoft Visual C++ runtime is not part of the Linux build.

---

## Online services

The app looks data up at online services only when you ask it to. Their
data stays under their own terms:

- **Discogs** - This application uses Discogs' API but is not affiliated
  with, sponsored or endorsed by Discogs. 'Discogs' is a trademark of Zink
  Media, LLC.
- **Apple iTunes Search API** - the Radio tab's track covers. Shown only
  together with a link to the track on Apple Music, and never saved to a
  file, as Apple's terms require. A radio recording's cover file comes
  from MusicBrainz and the Cover Art Archive instead.
- **MusicBrainz** and **Cover Art Archive**, **radio-browser.info**,
  **GnuDb**, **ListenBrainz** and **Last.fm** (with your own account) - under
  their own terms of use.

---

Questions about a specific component's license terms: the component's own
project page is authoritative - this file is a snapshot of the versions
bundled with this build.
