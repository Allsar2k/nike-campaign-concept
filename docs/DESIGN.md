# Design system · Night Run

**Thesis:** *It should look like 7 p.m. on a Tuesday: streetlights, reflective strips, a group about to set off.* Most run clubs meet after work, in the dark. The visuals are black, with volt and orange the way safety gear catches the light.

## Palette

Defined once in [`assets/tokens.json`](../assets/tokens.json); `scripts/check-contrast.mjs` checks every pairing against WCAG 2.2 AA on each push.

| Token | Hex | Use | Contrast on `bg` |
|---|---|---|---|
| `bg` | `#0B0B0C` | Night background | — |
| `surface` | `#18181B` | Cards | — |
| `line` | `#2E2E33` | Borders and grid lines | decorative only |
| `ink` | `#F7F7F2` | Headlines and body text | 18.3:1 |
| `ink2` | `#B4B4AC` | Secondary text | 9.4:1 |
| `volt` | `#D4FF3A` | Primary highlight, buttons, the target segment | 17.0:1 |
| `onVolt` | `#0B0B0C` | Text on volt | 17.0:1 |
| `signal` | `#FF6A2B` | Second highlight, used sparingly for "now" and launch moments | 6.9:1 |

**Rule:** volt marks *the thing we chose* (the target segment, the open space on the map, the launch week). If everything is volt, nothing is.

## Type

- Headlines: heavy, condensed, uppercase, slightly slanted for forward motion (`'Arial Narrow'`, `'Helvetica Neue'` condensed, then Arial; `font-style: italic`, weight 800).
- Body: the system sans at normal width for readability. The motion is in the headlines, not the paragraphs.
- Tracking: tight on headlines (-0.01em), wide on labels (0.14em).

## Graphic language

- **Pace lines:** three slanted stripes, the visual signature, used in the banner and as section dividers.
- Hard corners (4px radius). This is a track, not a cloud.
- Charts mark the chosen option with volt plus a label and a heavier outline, never with colour alone.

## Graphics

| File | Shows |
|---|---|
| `assets/banner.svg` | Campaign banner: "Show Up" over pace lines |
| `assets/segmentation.svg` | The four segments by motivation and commitment |
| `assets/competitive-map.svg` | Brands by message and price, with the open space marked |
| `assets/channel-rollout.svg` | Six channels across 12 weeks |
