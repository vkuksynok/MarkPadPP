# Getting started with MarkPad++

MarkPad++ is a Markdown editor and viewer for Windows. This page covers installing
it, opening a `.md` file, working with tabs, and switching between the source and
the rendered reader mode.

## How do I install MarkPad++?

Install it from the Microsoft Store, at
https://apps.microsoft.com/detail/9PCKKT5MKL4L — the recommended channel, where
updates arrive automatically. A direct installer is also available from the
[GitHub Releases page](https://github.com/vkuksynok/MarkPadPP/releases/latest)
(updates are manual with that option). You need Windows 10 version 1809 (build
17763) or newer, or Windows 11, on x64.

## How do I open a Markdown file?

Open a `.md` file in any of these ways:

- **File › Open** from the menu.
- **Drag and drop** the file anywhere onto the window — the editor included. You can
  drop several files at once, and each opens in its own tab.
- **From the command line**, passing one or more file paths; each opens in a tab.
- **File › Open Recent**, which lists the last ten files opened or saved, most
  recent first. An entry that has since been moved or deleted drops off the list
  instead of staying there to fail again.

Opening a file that is already open brings its tab forward rather than opening a
second copy. Files are always read and written as UTF-8.

## Working with tabs

Every open file gets a tab, as in Notepad++.

- Each tab keeps its own text, undo history, caret and place in the document.
- An unsaved tab is marked with a `*`.
- Reorder tabs by dragging them.
- Close a tab with its `×`, a middle click, or `Ctrl+W`.
- Right-click a tab for *Close*, *Close Others*, *Close All* and *Copy Full Path*.
- Closing the last tab leaves an empty tab rather than an empty window.
- Quitting asks about each modified file in turn.

MarkPad++ runs as a single instance: opening a file adds a tab to the existing
window rather than launching another application window.

## Reading rendered Markdown (reader mode)

Press `Ctrl+E` to toggle reader mode. The document is rendered in place using the
current theme, so there is no split pane to manage — the editor and reader are the
same space.

Reader mode keeps your place: it opens at whatever the editor was showing, and
scrolling the reader and coming back moves the editor to match. Toggling without
scrolling leaves the editor exactly where it was. `Ctrl+C` copies from whichever
view is showing, so you can copy rendered text out of reader mode without the
Markdown punctuation.

The find bar is unavailable in reader mode, because searching applies to the
Markdown source. See [Keyboard shortcuts](keyboard-shortcuts.md) for the full list,
and [Exporting](exporting.md) for saving to PDF, Word or ODT.

## Themes

Switch between the built-in light and dark themes with **View › Theme**. A theme
drives the whole application: the window, menus, toolbar, editor and gutter, the
Markdown tokens in the editor, the rendered page, and the native Windows title bar.
User-supplied theme files are not supported in this release.
