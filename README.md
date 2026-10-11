# Ptero Skin

A browser extension that restyles the [Bot-Hosting.net](https://bot-hosting.net) dashboard to look like the classic Pterodactyl panel.

> **Unofficial.** This project is not affiliated with, endorsed by, or sponsored by Bot-Hosting.net or the Pterodactyl project. It only changes how the site looks in your own browser.

## Features

- Pterodactyl-style theme for the dashboard and server pages
- Toggle individual parts of the interface on or off
- Built-in presets: **Classic Pterodactyl**, **Compact**, **Minimal**, **Wide console**
- Save your own settings as named profiles
- Export and import your settings as a JSON file
- Changes apply live to open Bot-Hosting.net tabs

### Customisable options

| Area | Options |
| --- | --- |
| Top bar | Billing/Credits links, Assistant (AI) buttons |
| Dashboard | Plan details, "New deployment" tile, full-size or compact rows, status text on server cards, reorder handles, server sorting (manual, name A–Z, running first) |
| Server page | Stat tiles beside or below the console, Kill button, larger console text, full-width page |

## Install

### Firefox

1. Download the latest signed `.xpi` file from [zillies.dev/ptero-skin](https://zillies.dev/ptero-skin/0.3.1/PteroSkin-0.3.1.xpi).
2. Open the file in Firefox, or drag it onto a Firefox window, and confirm the install.

The extension updates itself automatically from the `updates.json` found on [zillies.dev](https://zillies.dev/ptero-skin/updates.json).

If the skin doesn't appear on Bot-Hosting.net, open `about:addons`, select the extension, go to **Permissions**, and allow access to the site.

### Chrome and other Chromium browsers

Install from the Chrome Web Store [here](https://chromewebstore.google.com/detail/pterodactyl-skin-for-bot/ncckbgmiecommbehpcpmihkmphnepmgg?authuser=0&hl=en)

1. Click the Chrome Web Store link and add the extension to Chrome.
2. Go to your Extension Manager and click "Pterodactyl Skin for Bot-hosting.net", it should be enabled by default.
3. Visit Bot-hosting.net and navigate to the dashboard, if the skin doesn't load, hard refresh the page and it should apply.

## Usage

Click the extension icon to open the settings panel. From there you can:

- Turn the skin on or off with **Enable skin**
- Pick a preset and click **Apply preset**
- Adjust individual options
- Save the current settings as a profile, and load or delete profiles later
- Export or import a backup of your settings
- Reset options to their defaults, or clear the saved server order

Changes apply to open tabs. If a tab doesn't update, refresh the page.

## Privacy

- The extension runs only on `bot-hosting.net` and its subdomains.
- It stores your settings using the browser's extension storage (`storage` permission). Nothing is sent anywhere.
- It collects no data and makes no network requests of its own.

## Development

The extension is plain JavaScript and CSS with no build step required.

| File | Purpose |
| --- | --- |
| `manifest.json` | Extension manifest |
| `content.js` | Content script that applies the skin to the page |
| `pterodactyl.css` | The theme stylesheet |
| `options.js` | Option definitions, presets and settings helpers |
| `panel.html`, `panel.js`, `panel.css` | Settings panel |
| `icons/` | Extension icons |

## Contributing

Bug reports and suggestions are welcome. Please open an issue. Bot-Hosting.net can change its page layout at any time, so when something looks broken, a screenshot and the page URL help a lot.

## License

Copyright (c) 2026 zilly-js. All rights reserved.

You may install and use Ptero Skin for yourself. You may not redistribute it, or upload it or any modified version of it to any extension store or other site, without permission. See LICENSE for the full terms.

To ask for permission, open an issue.
