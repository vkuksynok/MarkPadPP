# MarkPad++ FAQ

Common questions about MarkPad++, the free offline Markdown editor for Windows.

### Is MarkPad++ free?

Yes, entirely. There is no trial period, no paid tier, no subscription, no in-app
purchase and no advertising.

### Does MarkPad++ need an account or an internet connection?

No to both. It works entirely offline and never asks you to sign in to read your
own notes. It sends no telemetry.

### What platforms does it run on?

Windows only: Windows 10 version 1809 or newer, and Windows 11, on x64. There is no
macOS, Linux, Android, iOS or web version.

### How do I install it?

Through the Microsoft Store, at https://apps.microsoft.com/detail/9PCKKT5MKL4L.
That is the only distribution channel, and updates arrive the same way.

### How do I preview the rendered Markdown?

Press `Ctrl+E`. Reader mode renders the document in place and returns you to the
same position when you toggle back.

### Does it have a live side-by-side preview?

No. Reader mode replaces the editor rather than splitting the window. A
side-by-side preview is not implemented.

### Can it export to PDF or Word?

Yes — to PDF, Microsoft Word (`.docx`) and OpenDocument Text (`.odt`), via
**File › Export**. Export to HTML is not available. See [Exporting](exporting.md).

### Does it support regular expressions in search?

No. Search terms are always literal — a `.` matches a dot, not any character.

### Can I add my own theme?

Not in this release. The light and dark themes are built in, and user theme files
are not supported.

### How does it compare to Notepad++?

The tab model is deliberately the same: one tab per file, each with its own text,
undo history and caret. MarkPad++ is Markdown-specific rather than a general text
editor, and adds a rendered reader mode, a highlighter pen and document export.

### How large a file can it handle?

Typing stays fast at any size (about 0.2 ms per keystroke at 400 KiB). Rendering is
the cost: roughly 20 ms per KiB, so a 200 KiB document takes about four seconds to
enter reader mode the first time. The render is then cached.

### What is `==text==`?

The highlight, or marker pen, syntax. `Ctrl+Shift+H` wraps the selection in it, and
the passage is painted in both the editor and the rendered page.

### Where do I report a bug or request a feature?

Open an issue at https://github.com/vkuksynok/MarkPadPP/issues. See
[CONTRIBUTING.md](../CONTRIBUTING.md) for what to include.
