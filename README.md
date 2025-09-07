# Chrome Tabs Recovery

Recover lost Chrome tabs by extracting URLs from Chrome’s internal `tabs` file. Runs fully in your browser; no data leaves your machine.

## Quick Start

1. Open `index.html` in a modern browser.
2. Drag and drop your Chrome `tabs` file, or click “Choose File”.
3. Review recovered URLs. Expand “Best of …” to see alternatives. Export or open tabs as needed.

## Find Your `tabs` File

- Windows: `C:\\Users\\<you>\\AppData\\Local\\Google\\Chrome\\User Data\\Default\\tabs`
  - Also check: `...\\Default\\Sessions\\tabs_*`
- macOS: `~/Library/Application Support/Google/Chrome/Default/tabs`
- Linux: `~/.config/google-chrome/Default/tabs`

Tip: If you use multiple profiles, check `Profile X` folders and pick the most recently modified file.

## Features

- Local-only processing (privacy-friendly)
- Drag & drop or file picker
- Deduplication and cleanup of noisy entries
- Instant search and domain grouping
- Export: HTML report, browser bookmarks, JSON
- “Open All” to restore tabs (use with care)

## Troubleshooting

- “No URLs found”: Verify you selected the correct `tabs` file; try the `Sessions/tabs_*` files; ensure file size > 1KB.
- Can’t find file: Show hidden folders; check other profiles (`Profile X`); use the most recent file.
- Many invalid/partial URLs: Source file may be corrupted; try an older `tabs`/`tabs_*` file.

## Development

- Single-file app: edit `index.html` and open it in a browser to test.
- Contributions are welcome via issues or pull requests.

## Privacy

- No uploads, tracking, or storage. Everything runs locally in your browser.

## License

MIT

