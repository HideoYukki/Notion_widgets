# Free Notion Widgets

Ready-to-use widgets for Notion. No sign-up, no coding: copy the link, paste it, done.

## Widgets

| Widget | Description | Link |
|--------|-------------|------|
| 🌤️ Weather | 3-day forecast, auto-detects city, language and units | `https://hideoyukki.github.io/widgets/embed/weather/` |
| 🕐 World clock | Live clocks for up to 8 cities with day/night icons. Pick cities via `?cities=Name\|Europe/Zone`. | `https://hideoyukki.github.io/widgets/embed/clock/` |
| 🖼️ Parallax image | Fits any image to the block and adds a smooth parallax effect. Set it via `?src=IMAGE_URL`. | `https://YOUR_USERNAME.github.io/REPO_NAME/embed/parallax/?src=IMAGE_URL` |

## Colors

Add parameters to any widget link (hex without `#`): `color` (background), `text` (optional), `accent` (optional).

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