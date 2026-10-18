# Mercury faceplate: final dimensions

All dimensions in mm. Front view (labels facing you).
X is measured from the left edge, Y from the top edge.

## Plate

- 20 wide × 177 tall (bottom edge moved down 0.5 from the measured 176.5)

## Screw slots (Ø3.5 × 0.5 slack)

Each hole is a slot: the top semicircle is at the center below, the bottom semicircle is 0.5 mm lower, joined by straight sides (3.5 wide × 4.0 tall overall).

| Slot   | X (center) | Y (top-semicircle center) | Notes                 |
|--------|-----------:|-----------:|-----------------------|
| Top    | 11.5       | 4.5        | 4.5 from top edge     |
| Bottom | 11.5       | 171        | 6 from bottom edge    |

Hole centers are 166.5 apart (166 measured on the unit; bottom hole moved down 0.5).

## Rectangular cutouts

| Cutout  | X           | Y            | Size (W × H) | Center (X, Y) |
|---------|-------------|--------------|--------------|---------------|
| OPT OUT | 5.5 – 15.5  | 43.5 – 53.5  | 10 × 10      | 10.5, 48.5    |
| OPT IN  | 5.5 – 15.5  | 59.0 – 69.0  | 10 × 10      | 10.5, 64.0    |
| PCM OUT | 2.2 – 14.5  | 74.5 – 102.0 | 12.3 × 27.5  | 8.35, 88.25   |

Key relationships:

- OPT OUT center: 44 below the top hole center
- OPT IN center: 15.5 below the OPT OUT center
- PCM OUT center: 24.25 below the OPT IN center (24.5 was measured; 0.25 is within measurement error)
- Optical cutout centers: 9.5 from the right edge (the optical jacks sit lower on the PCB than the RCA jacks)
- PCM OUT: 2.2 strip on its left side, center 11.65 from the right edge

All cutout corners: R0.5 (for strength at the 2.2 strip; intrudes only ~0.2 along each corner diagonal).

The CTRL and OPN3-L cutouts from the reference photo are omitted; this unit doesn't have them.

## Labels

Helvetica Neue Medium, converted to outlines. Each label sits to the right of its cutout, reads bottom to top (letter tops face the cutout), and is centered on the cutout's Y.

| Label   | Font size | Cap height | Baseline X | Length |
|---------|----------:|-----------:|-----------:|-------:|
| OPT OUT | 2.6       | 1.86       | 18.8       | 11.25  |
| OPT IN  | 2.6       | 1.86       | 18.8       | 8.3    |
| PCM OUT | 3.1       | 2.21       | 18.45      | 14.1   |

Sizes and positions were matched to the lettering in a photo of an original cover (±0.3).

## Provenance and accuracy

- Positions: measured on the unit, ±0.5.
- Cutout sizes: inferred from a dewarped photo, ±0.5. Check them against the real connectors.
- Hole countersinks: not determined; drawn as plain holes.

## Before cutting

1. Print `faceplate.svg` at 100% (no fit-to-page). Verify that the plate is 177 and the holes are 166.5 apart.
2. Hold the paper template against the card's connectors.
3. If any fit is tight, add ~0.3 clearance per side to that cutout.
4. The 2.2 strip beside PCM OUT bends easily, so cut it last or support it.

## Files

- `faceplate.dxf`: R12, mm, origin at the bottom-left (Y up); layers OUTLINE / CUTOUTS / HOLES / TEXT; cutouts are lines + R0.5 arcs; text is closed polylines (glyph outlines, counters included)
- `faceplate.svg`: 1:1, mm, origin at the top-left
