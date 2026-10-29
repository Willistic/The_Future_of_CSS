# Control Deck

A sci-fi cockpit built in pure CSS (no JavaScript) to preview features from the
[Interop 2027 shortlist].

| Feature | Where |
|---|---|
| `@function` | `--polar()` places orbiting radar blips, `--glow()` shares shadows |
| `corner-shape` | bevel / notch / scoop / squircle module corners |
| `border-shape` | hero hull outline that morphs on hover |
| Anchored container queries | tooltip caret flips with the fallback position |
| Scroll-triggered animations | power-up sequence modules |
| `reading-flow` | tab order follows the grid when you hit **Reflow layout** |
| `interpolate-size` | subsystem drawers animate to `height: auto` |
| Gap decorations (`rule`) | schematic lines between modules |
| Scroll-state container queries | status bar "stuck" style, log scroll fades |

The status bar shows live green/red lights for each feature via `@supports`.

## Run

No build step. Open `index.html`, or serve the folder:

```sh
python3 -m http.server 5173
```

Use Chrome 155+ / Edge 154+ for the full effect. Other browsers get plain
rounded corners, normal borders and no scroll animations.

Note: the experimental syntax (`border-shape`, `timeline-trigger`, gap
decorations) is still moving; property names may need tweaks as specs settle.
