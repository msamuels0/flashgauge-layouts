# FlashGauge Layouts site

Static GitHub Pages site for `layouts.flashgauge.com`.

## Structure

- `index.html` — public layout gallery/viewer
- `configurator/index.html` — FlashGauge Layout Studio (based on configurator v18)
- `layouts/` — published `.fglayout` bundles
- `layouts/layouts.json` — gallery manifest
- `CNAME` — custom domain for GitHub Pages

## Add a layout

1. Copy the `.fglayout` file into `layouts/`.
2. Add an entry to `layouts/layouts.json`, for example:

```json
{
  "layouts": [
    {
      "file": "retro-cafe-rev1.fglayout",
      "title": "Retro Cafe",
      "author": "FlashGauge",
      "description": "Classic round tach layout"
    }
  ]
}
```

The gallery reads the `.fglayout` file itself and renders the full preview in the browser. No separate preview image is required.

The **Open in configurator** button passes the hosted layout to `/configurator/`, where it is fetched and opened automatically.
