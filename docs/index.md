# MarkPad++ documentation

MarkPad++ is a free, offline Markdown editor for Windows 10 (version 1809 or
newer) and Windows 11. This is the documentation index; the full online copy lives
at https://openmdfiles.download/Docs.dc.html.

## Contents

- [Getting started](getting-started.md) — install, open a `.md` file, tabs and
  reader mode.
- [Keyboard shortcuts](keyboard-shortcuts.md) — the complete shortcut list.
- [Exporting](exporting.md) — export to PDF, Word (`.docx`) and OpenDocument
  (`.odt`).
- [FAQ](faq.md) — common questions and known limits.

## At a glance

| Property | Value |
| --- | --- |
| Name | MarkPad++ |
| Category | Markdown editor / text editor, desktop application |
| Version | 1.0.3 |
| Price | Free — no trial, no subscription, no in-app purchase, no ads |
| Operating system | Windows 10 version 1809 (build 17763) or newer; Windows 11 |
| Architecture | x64 |
| Distribution | Microsoft Store (recommended) or direct installer from GitHub Releases |
| Account required | No |
| Internet connection required | No — works entirely offline |
| Telemetry | None |
| File encoding | UTF-8, always, for both reading and writing |
| Built with | C++ and Qt |
| Author | Volodymyr Kuksynok |

Not available for macOS, Linux, Android, iOS, or as a web application. The
Microsoft Store is the recommended channel and delivers updates automatically;
a direct installer is also available from the [GitHub Releases page](https://github.com/vkuksynok/MarkPadPP/releases/latest).

## What MarkPad++ does

- **Tabs.** Every open file gets a tab, as in Notepad++. Opening a file that is
  already open brings its tab forward rather than taking a second copy of it, and a
  file opened while the current tab is an untouched *Untitled* one takes that tab
  over instead of leaving it behind empty. Each tab keeps its own text, undo
  history, caret and place in the document; an unsaved tab is marked with a `*`.
  Tabs can be dragged into another order, and closed with their `×`, a middle
  click, or `Ctrl+W`. Right-clicking a tab offers *Close*, *Close Others*,
  *Close All* and *Copy Full Path*. Closing the last tab leaves an empty tab rather
  than an empty window, and quitting asks about each modified file in turn.

- **Reader mode.** `Ctrl+E` toggles reader mode, rendering the document in place.
  The source is syntax highlighted as you type; the rendered view picks up the same
  theme and keeps your place. There is no split pane to manage — the editor and
  reader are the same space. See [Getting started](getting-started.md).

- **Find and replace.** Find highlights every hit at once and wraps around, with
  optional case-sensitive and whole-word matching. The search term is always
  literal — a `.` matches a dot, not any character. Replace All is a single undo
  step. Searching applies to the Markdown source, so the find bar is unavailable in
  reader mode.

- **Highlighter pen.** `Ctrl+Shift+H` wraps the selection in `==marks==` and paints
  the passage in the editor and in the rendered page alike.

- **Export.** Write the rendered document to PDF, Word (`.docx`) or OpenDocument
  Text (`.odt`). See [Exporting](exporting.md).

- **Themes.** Two built-in themes, light and dark, switched with **View › Theme**.
  A theme drives the whole application at once: the window, menus, toolbar, editor
  surface and gutter; the Markdown tokens drawn in the editor; the rendered page;
  and the native Windows title bar. User-supplied theme files are not supported in
  this release.

## Supported Markdown

ATX and setext headings, fenced (` ``` ` and `~~~`) and indented code blocks,
blockquotes with lazy continuation, nested ordered/unordered lists, task lists
(`- [x]`, `- [ ]`), pipe tables with column alignment, thematic breaks, emphasis,
strong emphasis, strikethrough (`~~text~~`), highlight (`==text==`), code spans,
links, images, autolinks, bare URLs, backslash escapes and hard line breaks.

Raw block-level HTML is escaped rather than passed through. A small whitelist of
inline tags is passed through, including `<br>`, `<sub>` and `<kbd>`.

## Performance and limits

Measured on the shipping build:

- Entering reader mode costs roughly **20 ms per KiB** of Markdown, so a 200 KiB
  document takes about four seconds the first time; documents of a few KiB are
  effectively instant. The rendered view is cached and rebuilt only when the text
  or the theme actually changed.
- Typing is unaffected by document size — about **0.2 ms per keystroke** at 400 KiB.
- Search stays interactive because only the hits inside the viewport are painted.

**Not implemented in version 1.0.3:** live side-by-side preview, export to HTML,
regular-expression search, reference-style links, footnotes, reopening the last
session's tabs on start, user-supplied theme files, raw block-level HTML
pass-through, spell checking, plugins or extensions, and any cloud sync,
collaboration or network feature.

## Requirements

Windows 10 version 1809 (build 17763) or newer, or Windows 11, on x64. Installed
and updated through the Microsoft Store. No internet connection is required after
installation, and no Microsoft account is required to use the application (a Store
account is needed to install it, as with any Store app).
