# Palanca Theme

A dark theme for Zed (and other editors), inspired by [Vesper](https://github.com/raunofreiberg/vesper).

## Screenshots

![Main Screenshot](./palanca-theme-screnshot-1.png)

![Variant 1](./palanca-theme-screnshot-transparent.png)

---

## Installation

You can install Palanca Theme in two ways:

### 1) Install via Zed Extensions (Marketplace)

1. Open Zed
2. Go to: Settings → Extensions (or press `Cmd + ,` on macOS and search for “Extensions”)
3. In the search bar, look for “Palanca Theme”
4. Click “Install”
5. Apply the theme: Settings → Themes → select “Palanca” (or use the “Zed: Select Theme” command)

> Tip: If it doesn’t show up immediately, check your connection, restart Zed, or refresh the extensions list. If the theme isn’t published yet, use the manual installation below.

### 2) Manual installation (without Marketplace)

If you want to use locally or test before publishing:

1. Close Zed (if it’s open)
2. Create the theme folder under Zed’s extensions (dev/local). On macOS:
   - `~/Library/Application Support/Zed/extensions/palanca-theme`
3. Copy the repository files into that folder (including the extension manifest and color scheme files)
4. Open Zed and enable the theme:
   - Settings → Themes → select “Palanca”
   - Or run “Zed: Select Theme” and choose “Palanca”

#### File structure (example)

Make sure to include at least:
- `extension.json` (manifest)
- `themes/palanca.json` (colors/styles)
- `README.md` (documentation)
- `icons/` (if you have a theme icon)
- `assets/` (if you have images/screenshots)

Minimal `extension.json` example:

```json
{
  "name": "palanca-theme",
  "display_name": "Palanca Theme",
  "description": "Dark theme for Zed, inspired by Vesper.",
  "version": "1.0.0",
  "author": "Clemilson Azevedo",
  "repository": "https://github.com/ClemilsonAzevedo/palanca-theme",
  "categories": ["Themes"],
  "themes": [
    {
      "name": "Palanca",
      "path": "themes/palanca.json"
    }
  ]
}
