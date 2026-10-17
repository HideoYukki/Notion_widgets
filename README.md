# Free Notion Widgets

Ready-to-use widgets for Notion. No sign-up, no coding: copy the link, paste it, done.

## Widgets

Use the **[configurator](https://hideoyukki.github.io/Notion_widgets/configurator)** to tweak a widget with a live preview and get a ready-to-paste link.

| Widget | Description | Link |
|--------|-------------|------|
| 🌤️ Weather | 3-day forecast, auto-detects city, language and units | `https://hideoyukki.github.io/Notion_widgets/embed/weather/` |
| 🕐 World clock | Live clocks for up to 8 cities with day/night icons. Pick cities via `?cities=Name\|Europe/Zone`. | `https://hideoyukki.github.io/Notion_widgets/embed/clock/` |
| 🏃 Progress platformer | A pixel-art character walks across a platformer level as the year (or month, week, day) passes. Background and outfit follow the time of day. | `https://hideoyukki.github.io/Notion_widgets/embed/progress/` |
| 🖼️ Parallax image | Fits any image to the block and adds a smooth parallax effect. Set it via `?src=IMAGE_URL`. | `https://hideoyukki.github.io/Notion_widgets/embed/parallax/?src={IMAGE_URL}` |

## Colors

Add parameters to the Weather and World clock links (hex without `#`): `color` (background), `text` (optional), `accent` (optional).

`.../embed/clock/?color=4E2B3C&accent=F2B8CF`

Without parameters, widgets follow the system light/dark theme.

## Customizing the Parallax image

Required: `src` (URL-encoded image link). Optional:

- `fit`: `cover` (default), `contain`, `fill`
- `pos`: focal point in %, e.g. `50,30`
- `strength`: 0–100 (default `30`)
- `mode`: `both` (default), `pointer`, `auto`, `off`
- `radius`: corner radius in px
- `bg`: letterbox for `contain`: `blur` (default), hex color, `none`

## Customizing the Progress platformer

All optional:

- `track`: `year` (default), `month`, `week`, `day`
- `hour`: force a time of day (0–24) instead of the live clock, e.g. `22`
- `radius`: corner radius in px
- `demo`: `1` shows a bar to switch the track and scrub the time of day

Coins mark the sub-periods (months, weeks, days or 3-hour steps) and disappear once collected. The widget uses your browser's clock and makes no network requests.

## How to add to Notion

1. On your Notion page, type `/embed` and choose **Embed**.
2. Paste the widget link and click **Embed link**.
3. Drag the bottom edge of the block to adjust its height.

## FAQ

**Is it free, and do I need an account?**
Yes, it's free. No, you don't need an account.

**The widget doesn't load in Notion.**
Check that the link works in a regular browser tab. If it does, refresh Notion or paste the link again. If it still fails, open an issue in **Issues**.

## Make your own copy

Click **Fork**, enable **Settings** → **Pages** in your copy (**Deploy from a branch**, `main`, `/ (root)`), and edit the files in `embed/{name}/index.html`.

## Privacy

Widgets don't store anything. Some connect to external services (e.g. Weather: Open-Meteo, ipwho.is, ipapi.co, BigDataCloud), which can see your IP address.