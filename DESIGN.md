# Lanterns: design notes

## Identity

*Lanterns* is a slow, dark detective story about two Green Lanterns in the American heartland, and its title sequence is a yellow lens inside a green ring. The theme takes that seriously: it is built from the show's objects, not from the franchise's bright green.

- **Should feel:** dark, quiet, physical, like old metal and glass under a single light; will and fear side by side.
- **Should not feel:** neon, superhero-bright, jade or spa-green, a rainbow terminal, a generic green theme.

## Thesis: every surface is an object

| Surface | Object | Treatment |
|---|---|---|
| Focused window | Hal's ring | Glint border: graphite → ring emerald → ring brass → graphite at 135°. Dark ends make it read as light catching metal. |
| Unfocused window | The ring in shadow | Dim brass at 60% opacity. |
| Bar | The ring's frame | Same graphite as the windows, brass lettering, so bar and window are one object. |
| Menu / launcher selection | The ring itself | 2px brass gradient frame, faint emerald enamel inside, text in the lit emerald of the stone. |
| Accent and icons | John's lantern glass | Olive green; Yaru-olive icons match it. |
| Unlock screen | The ring face | Flat vector of the ring on graphite. |

## Palette and provenance

Every value was measured from the wallpapers or from tone-mapped stills of the season, then pushed only as far as that colour's own peak saturation in the footage. Nothing is invented and nothing is lifted beyond the source.

| Role | Hex | Source |
|---|---|---|
| Ground | `#141412` | Near-neutral graphite; the darks of every frame. |
| Text | `#d1cab5` | Bone, from the brass highlights, lowered to 11.3:1 for long reading. |
| Dim text | `#89867c` | Ash. |
| Selection | `#0d4833` | The darkest emerald cluster across the set. |
| Green | `#009863` / `#24ba7d` | Ring emerald (peak chroma .17 in the ring's glow). |
| Accent / magenta slot | `#83b755` | Lantern glass (peak .14). No purple exists in the source. |
| Cyan | `#89d0aa` | The beacon's afterglow. |
| Blue | `#7db6bd` | Window steel: the sheen on the lantern body (peak .06). |
| Yellow (warnings) | `#d9cf63` | Title-sequence lens (peak .11). |
| Red slot (errors) | `#ee9b57` | Motel neon, the only warm light in the set. There is no red in the source, so there is none here. |
| Orange | `#9d8342` | Lantern brass in shadow. |
| Bar / frames | `#a6936b` | Ring brass, measured on the ring's frame. |

Slot names are only schema labels: red is neon, magenta is glass, blue is steel, cyan is the beacon. The palette clusters into two families, olive/lens and emerald, with brass and steel as neutral metals.

## Accessibility

Body text is 11.3:1, dim text 5.1:1, and every syntax colour clears 4.5:1 on the ground. For red-green colour blindness the error/green pair separates by lightness (dE 7.9). The weakest pair is brass vs emerald, accepted because brass is rarely used for text.

## Wallpapers

Rules the set follows:

- One frame per scene. No near-duplicates, no stills a few seconds apart.
- Objects and silhouettes, not faces in close-up.
- Raw frames only; cut-out objects on flat grounds do not belong in the set.
- Edits reuse the frame's own texture (the Omarchy title is filled with tiles of the original title's starfield), never synthetic grain.
- Order tells the story: the ring face, the opening titles, Hal, John, the night the season ends in.
- Golden-void frames were left out: their warm ochre fights the graphite ground.

## Guardrails

- Keep the ground graphite. Tinting it brown or green turns the theme into a different (and more generic) one.
- Keep green for the ring. If a new surface needs emphasis, reach for brass first.
- Do not add red, purple or pink; they are not in the source.
- New colours must be measured from the footage and stay within their family's peak saturation.
- The window border keeps its dark ends; a border without them loses the glint.
