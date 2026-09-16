# Exporting from MarkPad++

MarkPad++ can export the rendered Markdown document — without the Markdown
punctuation — to PDF, Microsoft Word or OpenDocument Text. Use **File › Export**.

## Which formats can MarkPad++ export to?

Three formats:

| Format | Extension |
| --- | --- |
| PDF | `.pdf` |
| Microsoft Word | `.docx` |
| OpenDocument Text (ODF) | `.odt` |

Export to HTML is **not** available in this release.

## How export behaves

- Formatting, tables, links and images are all carried into the exported file.
- Export uses a print-friendly light theme, regardless of the theme in use.
- Relative image paths are resolved beside the source Markdown file.
- Export does not change the open file or its modified state.

## How do I convert Markdown to PDF?

Open the `.md` file, choose **File › Export**, pick **PDF (`.pdf`)** as the format,
and choose where to save. The rendered document — headings, tables, links and
images included — is written out with a print-friendly light theme, and your open
file is left untouched.

The same steps produce a Word (`.docx`) or OpenDocument (`.odt`) file; just pick
that format instead.
