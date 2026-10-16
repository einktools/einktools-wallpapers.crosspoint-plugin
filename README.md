# einktools Wallpapers for CrossPoint

A CrossPoint plugin that browses the public-domain art gallery at [einktools.com/wallpapers](https://einktools.com/wallpapers) on your Xteink reader and saves pictures into your sleep-screen rotation.

- Every picture is cut to the exact screen size: 480×800 for X4 and X4 Pro, 528×792 for X3. No bars, no stretching.
- Pictures are pre-dithered to the 4 grays the panel shows, as 2-bit BMPs of about 100 KB.
- 60 plates (animals, botanicals, Japanese prints, machines, space and more), all public domain.

## Install with Plugin Hub

1. Use a CrossPoint build with the plugin system.
2. Open **Plugins**, launch **Plugin Hub**, refresh the Community catalog.
3. Install **einktools Wallpapers**.

## Install by hand

Copy the `einktools-wallpapers.crosspoint-plugin/` folder to `/plugins/einktools-wallpapers/` on the SD card.

## Use

1. Open the plugin, pick your model list and a picture. It is saved to `/.sleep`.
2. Settings > Sleep Screen > Custom. The reader picks a random picture from `/.sleep` each time it sleeps.

If `/sleep.bmp` exists it is shown instead of the `/.sleep` pictures. Delete or rename it to use the rotation.

Want your own photo instead? Make one at [einktools.com/xteink-wallpaper-converter](https://einktools.com/xteink-wallpaper-converter). It runs in your browser; the image never leaves your device.

## Layout

```text
einktools-wallpapers.crosspoint-plugin/   # installable payload (Plugin Hub standard)
├── manifest.json
├── device.json
└── README.md
```

The catalog and images are served from einktools.com. Downloading a picture sends no account or device data.
