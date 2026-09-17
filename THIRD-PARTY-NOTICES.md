# Third-Party Notices

**MarkPad++**

Last updated: 2026-09-17

MarkPad++ incorporates third-party components. Each component remains subject to
its own license terms, which prevail over the
[MarkPad++ End User License Agreement](EULA.md) in respect of that component.

Full license texts are included in the [`third-party-licenses/`](third-party-licenses/) directory of
this repository and are also distributed with the application.

---

## Qt Framework

- **Copyright:** © The Qt Company Ltd. and other contributors
- **Homepage:** https://www.qt.io/
- **License:** GNU Lesser General Public License, version 3
  ([`third-party-licenses/LGPL-3.0.txt`](third-party-licenses/LGPL-3.0.txt)), which incorporates the
  terms of the GNU General Public License, version 3
  ([`third-party-licenses/GPL-3.0.txt`](third-party-licenses/GPL-3.0.txt))
- **Modifications:** The Qt libraries distributed with MarkPad++ are unmodified
  binaries built from the official Qt sources.

> **TODO — заповнити перед комітом.** Внеси точну версію Qt і перелік
> модулів. Отримати список:
> `Get-ChildItem "<тека білду>" -Filter Qt*.dll | Select-Object Name`
> а версію — з властивостей будь-якого `Qt6*.dll` або з
> `qmake -query QT_VERSION`.

| Component | Version | License |
|---|---|---|
| Qt Core | | LGPL-3.0 |
| Qt GUI | | LGPL-3.0 |
| Qt Widgets | | LGPL-3.0 |

### Your rights under the LGPL

The LGPL-3.0 grants you certain rights in respect of the Qt libraries, which
MarkPad++ does not and cannot restrict:

- You may obtain the corresponding source code of the Qt libraries from
  https://download.qt.io/ or from The Qt Company.
- You may modify the Qt libraries and use MarkPad++ with your modified version.
- You may reverse engineer MarkPad++ to the extent necessary to debug such
  modifications.

MarkPad++ links against Qt **dynamically**. The Qt libraries are installed as
separate `.dll` files in the application directory, so relinking requires no
action on our part: replace the relevant `.dll` file with your own build of the
same Qt version and the application will load it.

If you require any further information or material that the LGPL-3.0 obliges us
to provide, contact volodymyr.kuksynok@gmail.com.

---

## MinGW-w64 Runtime Libraries

MarkPad++ is built with the MinGW-w64 toolchain and distributes its runtime
libraries (`libgcc_s_seh-1.dll`, `libstdc++-6.dll`, `libwinpthread-1.dll`).

- **libgcc / libstdc++** — © Free Software Foundation, Inc. Distributed under
  the GNU General Public License, version 3, **with the GCC Runtime Library
  Exception**, which permits distribution with software under any license.
  See https://www.gnu.org/licenses/gcc-exception-3.1.html
- **libwinpthread** — part of MinGW-w64, © the MinGW-w64 project, distributed
  under permissive MIT-style and BSD-style terms. See
  https://sourceforge.net/p/mingw-w64/mingw-w64/ci/master/tree/COPYING

---

<!-- Додай сюди решту, якщо щось із цього є у білді: KDE Syntax Highlighting
     (LGPL-2.1+), md4c (MIT), cmark / cmark-gfm (BSD-2-Clause), maddy (MIT),
     иконки чи шрифти (OFL / CC-BY). Кожен запис — назва, версія, копірайт,
     ліцензія, посилання на текст у third-party-licenses/. -->

## Reporting an omission

If you believe a component is used in MarkPad++ without proper attribution,
please open an issue at
https://github.com/vkuksynok/MarkPadPP/issues or write to
volodymyr.kuksynok@gmail.com, and it will be corrected.
