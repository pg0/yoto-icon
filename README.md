# Yoto Icon Maker

Browser tool to turn any image into a 16x16 PNG icon for the [Yoto player](https://yotoplay.com) display. Single HTML file, no dependencies, no build step, fully client-side - open `index.html` and go.

![Yoto Icon Maker](screenshots/skye.png)

## Features

- **Input**: file picker, drag & drop, or paste (Ctrl+V)
- **Crop & align**: drag to pan (also beyond the image edges), mouse-wheel / slider zoom 0.25x-5x, center reset
- **Background removal**: corner-seeded flood fill with tolerance slider
- **Pixelate**: grid sizes 16-128
- **Sampling modes**: Smooth (area average), Nearest, Dominant (most frequent color per cell), Median
- **Color reduction**: median-cut quantization to 4/8/16/32 colors, optional Floyd-Steinberg dithering
- **Background color**: optional solid fill behind the icon
- **Paint**: black / white / custom color / eraser brushes on the 16x16 grid, undo (Ctrl+Z), clear
- **Live preview**: original | 16x16 output | mockup on a Yoto Mini photo
- **Palette**: most-used colors with hex + share, click to copy
- **Export**: true 16x16 PNG with transparency, custom filename

## Why 16x16?

The Yoto player renders icons at 16x16 physical pixels. The tool processes and exports at exactly that resolution, so what you see in the output panel is what the device shows.

## Usage

Open `index.html` in any modern browser. Everything runs locally; no image ever leaves your machine.

## License

MIT
