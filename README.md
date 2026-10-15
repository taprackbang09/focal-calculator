# Focal Length Calculator

A small single-page calculator for choosing a camera lens. Enter a sensor size and the desired field of view (FOV), and it computes the required lens focal length. It includes an SVG diagram of the geometry and presets for common thermal camera sensors.

**Live page:** https://taprackbang09.github.io/focal-calculator/

## Formula

```
f = d / (2 · tan(FOV / 2))
```

- **f** — lens focal length (mm)
- **d** — sensor dimension along the FOV axis (mm): width for horizontal FOV, height for vertical FOV, or diagonal for diagonal FOV
- **FOV** — desired field of view (angle) along that same axis

## Thermal sensor size

A thermal sensor's physical size is its pixel count multiplied by its pixel pitch:

```
size = pixels × pitch
```

For example, a 640×512 sensor with a 12 µm pitch is 640 × 0.012 = **7.68 mm** wide and 512 × 0.012 = **6.144 mm** high.

## Usage

No build step and no dependencies: just open `index.html` in a browser.
