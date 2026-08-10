# SPEC.md — Factual building specification extracted from the CAD set

**Source drawings** (all A4 portrait, single page, vector, no embedded text layer):
`Facade.pdf`, `ground_floor.pdf`, `first_floor.pdf`, `roof_and_second_floor.pdf`, `landscape.pdf`

**Method.** Every PDF was rasterised at 200 DPI (and locally at 300–600 DPI) and inspected
visually. In addition, the vector geometry was extracted directly from the PDF content
streams, so most values below are *exact drawing geometry*, not pixel estimates.

**Scale calibration** (derived, then verified against every printed dimension on each sheet):

| Sheet | Scale | Verification |
|---|---|---|
| `landscape.pdf` | 33.108 pt/m | all 20 printed dimensions reproduce exactly |
| `ground_floor.pdf` | 42.95 pt/m | all 22 printed dimensions reproduce exactly |
| `first_floor.pdf` | 48.35 pt/m | all 11 printed dimensions reproduce exactly |
| `roof_and_second_floor.pdf` | 45.49 pt/m | all 3 printed dimensions reproduce exactly |
| `Facade.pdf` | 46.198 pt/m | **derived**, see §7 — no dimension lines on this sheet |

**Coordinate system used throughout this document**

- `X` = 0.00 at the **left** outer face of the building, increasing to the **right**, looking at the front facade.
- `Y` = 0.00 at the **rear** outer wall, increasing **towards the street**; the front facade line is `Y = 12.50`.
- `Z` = 0.00 at **ground-floor finished floor level (FFL)**. Front garden grade is `Z = −1.00`.
- Sheets were registered to one another using the 0.40 × 0.40 m structural columns, which
  coincide exactly on the ground, first and second-floor plans. This registration is
  **exact**, not estimated.

> **Reading the flags.** Values marked ✅ are read from a dimension line or are exact
> drawing geometry. Values marked ⚠️ **MEASURED** were computed from calibrated geometry
> but are **not** annotated on any drawing. Values marked ❓ **UNCERTAIN** are drawing
> ambiguities that a human should resolve. **No dimension in this document was invented.**

---

## 1. Site (`landscape.pdf`)

| Item | Value | Source |
|---|---|---|
| Plot shape | Irregular quadrilateral, near-rectangular, slight skew on the rear boundary | ✅ geometry |
| Plot front width (street boundary) | 11.13 m | ⚠️ MEASURED |
| Plot rear width | 10.88 m | ⚠️ MEASURED |
| Plot depth (right boundary) | 23.53 m | ⚠️ MEASURED |
| Plot depth (left boundary) | 23.09 m | ⚠️ MEASURED |
| Approx. plot area | ≈ 256 m² | ⚠️ MEASURED |
| Building footprint | 8.30 m × 12.50 m | ✅ dimensioned `8.30`, `12.50` |
| Left side yard | 1.01 – 1.26 m (tapers, boundary is skewed) | ⚠️ MEASURED |
| Right side yard | 1.57 m at ground floor | ⚠️ MEASURED |
| Rear yard | 1.51 – 1.95 m (tapers) | ⚠️ MEASURED |
| **Front yard depth** | **9.08 m** from front facade (Y 12.50) to street boundary (Y 21.58) | ⚠️ MEASURED |
| Front terrace strip | **2.00 m** deep, front wall to pool head | ✅ dimensioned `2.00` |

### 1.1 Pool

| Item | Value | Source |
|---|---|---|
| Pool size | **3.50 m × 5.50 m** | ⚠️ MEASURED (no dimension line; exact geometry of the filled water panel) |
| Pool position | `X 0.00 → 3.50`, `Y 14.50 → 20.00` | ⚠️ MEASURED |
| Relation to house | Left-aligned with the left elevation; leading edge 2.00 m in front of the facade | ✅ / ⚠️ |
| Relation to plot | ≈ 1.10 m off the left boundary; ≈ 1.58 m clear to the street boundary | ⚠️ MEASURED |
| Pool is drawn as | A plain rectangle of water with a graded blue fill; **no coping, steps, deck detail or plant is drawn** | ✅ observation |

### 1.2 Parking court

| Item | Value | Source |
|---|---|---|
| Parking court width | **3.65 m** (`X 4.65 → 8.30`) | ✅ dimensioned `3.65` |
| Cars shown | **2**, side by side, nose-in towards the house | ✅ observation |
| Car symbol size | 1.60 m × 4.42 m each | ⚠️ MEASURED |
| Car zone | `Y 16.16 → 20.58`, i.e. 3.66 – 8.08 m in front of the facade | ⚠️ MEASURED |
| Note | The two 1.60 m car symbols are drawn wider than the 3.65 m dimensioned court; the court reads as a **two-bay open forecourt**, not a garage. There is **no garage door and no carport structure** on any drawing. | ❓ minor drawing conflict |

### 1.3 Approach

- Entrance steps: **1.55 m wide** (`X 4.65 → 6.20`), 3 treads @ 0.35 m going,
  `Y 14.22 → 15.27`. ⚠️ MEASURED
- Entrance platform / plinth: from the steps up to the front wall, `Y 12.50 → 14.22`. ⚠️ MEASURED
- Front-left corner: a 0.40 m wide × 1.00 m long wall fin projects forward of the facade. ✅ dimensioned `1.00`
- Front-right corner: an L-shaped low wall, `X 6.55 → 8.10`, projecting 1.10 m forward. ✅ dimensioned `1.10`, `3.45`, `3.25`
- No street gate, fence, kerb, tree, planting or paving pattern is drawn anywhere on the site plan. ✅ observation

---

## 2. Levels and massing overview

| Level | Extent | Notes |
|---|---|---|
| Ground floor | 8.30 × 12.50 m full footprint (right-hand entrance block runs 0.50 m further forward, to `Y 13.00`) | ✅ |
| First floor | Same footprint **plus** a 4.95 × 1.80 m balcony projecting forward, **plus** a 0.80 m stair strip on the right flank, **plus** a 1.30 m strip at the rear | ✅ geometry |
| Second floor | Single **setback penthouse room 6.30 × 4.90 m** | ✅ dimensioned `6.30`, `4.90` |
| Roof | Large front roof terrace + side terrace + rear terrace wrapping the penthouse | ✅ |

**Number of levels: 3 occupied levels (G + 1 + setback 2nd) over a 1.00 m plinth, with an
accessible roof terrace at second-floor level.**

### 2.1 Setbacks of the penthouse (second floor)

| Direction | Setback | Source |
|---|---|---|
| From the **front** facade line (Y 12.50) | **3.20 m** (penthouse front wall at `Y 9.30`) | ⚠️ MEASURED |
| From the **rear** wall line (Y 0.00) | **4.10 m** (penthouse rear wall at `Y 4.10`) | ⚠️ MEASURED |
| From the **left** elevation | 0.14 m — effectively flush | ⚠️ MEASURED |
| From the **right** elevation (X 8.30) | **1.71 m**; the side roof terrace strip between penthouse and the stair is dimensioned **1.55 m** | ✅ dimensioned `1.55` |

### 2.2 Shape of the roof terrace

The roof terrace is a **stepped C / inverted-L wrapping the penthouse on three sides**:

- **Front terrace** (the big one): from the penthouse front wall `Y 9.30` to the parapet.
  The parapet is at `Y 12.50` for `X 0.00 → 4.64`, then **steps forward to `Y 14.30`** for
  `X 4.80 → 9.59` — i.e. the roof slab **runs out over the first-floor balcony below**.
  Front terrace ≈ 3.20 m deep on the left half, ≈ 5.00 m deep on the right half. ⚠️ MEASURED
- **Side terrace**: a 1.55 m wide strip down the right flank of the penthouse. ✅
- **Rear terrace**: ≈ 4.10 m deep across the full 8.30 m width, extending a further 1.30 m
  beyond the rear wall line. ⚠️ MEASURED
- Parapets are drawn as a 0.15 m thick line all round. No parapet **height** is given
  anywhere. ❓ height unknown

---

## 3. Ground floor — room schedule

Front facade is at the bottom of the plan. Rooms listed rear → front.

| # | Room | Size (m) | Position | Source |
|---|---|---|---|---|
| G1 | **Kitchen** (unlabelled; identified by the yellow counter run drawn as a U along three walls) | **3.55 × 4.35** | rear-left, `X 0.15–3.70`, `Y 0.15–4.50` | ✅ dims `3.55`, `4.35`; ❓ *name inferred from the counter symbol, not labelled* |
| G2 | **WC** | **1.30 × 2.45** | rear-centre, `X 3.85–5.15`, `Y 0.20–2.65` | ✅ dims `1.30`, `2.45`, labelled |
| G3 | **Bedroom** | **3.00 × 4.20** | rear-right, `X 5.15–8.15`, `Y 0.15–4.35` | ✅ dims `3.00`, `4.20`, labelled |
| G4 | **Living / main volume** (unlabelled) | **6.65 × 7.80** | the entire front-left half, `X 0.15–6.80`, `Y 4.50–12.30` | ✅ dims `6.65`, `7.80` |
| G5 | **Stair** | 1.10 m wide shaft, `X 6.80–7.90`, `Y ≈4.50–10.40`; 13 treads @ 0.263 m going, straight flight running rear→front | ⚠️ MEASURED |
| G6 | **Entrance hall** (unlabelled) | ≈ 1.75 × 1.90, `X 5.05–6.55`, `Y 10.40–12.30`, bounded left by a 1.90 m pier | ✅ dims `1.90`, `1.50` |
| G7 | **WC 2** | **1.45 × 2.30** | front-right, `X 6.70–8.15`, `Y 10.55–12.85` | ✅ dims `1.45`, `2.30`, labelled |

**Rooms sitting immediately behind the front elevation (ground floor), left to right:**
`Living (G4)` behind the big glazed panel → `Entrance hall (G6)` behind the door →
`WC 2 (G7)` behind the dark right-hand panel.

### 3.1 Ground floor openings

| Opening | Width | Position | Source |
|---|---|---|---|
| **Front glazing (living)** | **4.25 m** clear, split into 2 leaves at `X 2.45` (2.05 + 2.20 m); drawn as a 3-line sliding/double-glazed run | `X 0.40 → 4.65`, in the wall `Y 12.30–12.50` | ⚠️ MEASURED |
| **Entrance door** | 1.50 m structural opening; **1.20 m single leaf** shown swung open into the hall | `X 5.05 → 6.55` | ✅ dim `1.50`; leaf ⚠️ MEASURED |
| WC 2 door | 0.90 m | `X 6.65–7.55` at `Y 10.65` | ⚠️ MEASURED |
| Bedroom door | 1.00 m | right-hand end of the corridor wall | ⚠️ MEASURED |
| Rear kitchen window | 1.80 m (split at 2.45) | `X 1.00 → 2.80`, rear wall | ⚠️ MEASURED |
| Rear bedroom window | 2.00 m (split at 6.60) | `X 5.60 → 7.60`, rear wall | ⚠️ MEASURED |

---

## 4. First floor — room schedule

| # | Room | Size (m) | Position | Source |
|---|---|---|---|---|
| F1 | **Bedroom** (left) | **3.05** clear width beside a 0.50 m fitted wardrobe run; room 3.55 × 4.50 overall | rear-left, `X 0.15–3.70`, `Y 0.15–4.50` | ✅ dims `3.05`, `4.50` |
| F2 | **Bedroom** (right) | ≈ 2.95 × 4.20, with a 1.40 × 2.10 ensuite/closet at `X 3.85–5.25`, `Y 0.15–2.25` and a fitted wardrobe | rear-right, `X 5.20–8.15` | ⚠️ MEASURED (only `4.50` and `3.05` are dimensioned on this floor's rear half) |
| F3 | **Bathroom** | **2.20** wide × 1.24 deep | `X 0.15–2.35`, `Y 4.36–5.60` | ✅ dim `2.20`; depth ⚠️ MEASURED |
| F4 | **TV Room** | **6.06 × 3.55** | `X 0.15–6.21`, `Y 5.76–9.30` | ✅ dims `6.06`, `3.55`, labelled |
| F5 | **Void** (double-height over the living room) | **4.50 × 3.00** | `X 0.15–4.65`, `Y 9.30–12.30` | ✅ dim `3.00`; width 4.50 ⚠️ MEASURED |
| F6 | **Bar** | **3.50 × 3.45** | front-right, `X 4.65–8.15`, `Y 8.91–12.35` | ✅ dims `3.50`, `3.45`, labelled |
| F7 | **Balcony** | **4.95 × 1.80** | `X 4.65 → 9.60`, `Y 12.51 → 14.31` | ✅ dims `4.95`, `1.80`, labelled |
| F8 | Stair (upper flights) | main flight `X 6.80–7.90`; a second 0.80 m flight in a strip at `X 8.30–9.10`, `Y 4.71–8.91` | ❓ see §6 |

Overall front-to-back dimension of the bar + balcony zone: **5.40 m** ✅ dimensioned.

### 4.1 The double-height void — what it means for the elevation

The void (`X 0.15–4.65`, `Y 9.30–12.30`, 4.50 × 3.00 m) sits **directly behind the
front-left glazing**, over the front third of the ground-floor living room. Consequence:

> **The left-hand bay of the front facade is a single double-height glazed opening
> 4.25 m wide and ≈ 6.76 m tall, uninterrupted by a floor slab.** The first floor does not
> come forward to the facade in this bay — the TV Room stops 3.00 m short of it, and the
> void is open to the living room below.

Note a real conflict in the drawings, flagged and **not** reconciled by invention:
the glazed opening is **4.25 m** wide at ground level (`X 0.40–4.65`) but **3.65 m** wide
at first-floor level (`X 0.70–4.35`), whereas the elevation draws it as **one flush
4.25 m panel** full height. ❓ **UNCERTAIN — plan/elevation conflict.**

### 4.2 First floor openings

| Opening | Width | Position | Source |
|---|---|---|---|
| Front glazing, upper part of the double-height opening | 3.65 m | `X 0.70 → 4.35` | ⚠️ MEASURED |
| **Bar / balcony glazed door** | **1.80 m**, drawn as 2 leaves | `X 5.50 → 7.30` | ⚠️ MEASURED |
| Rear bedroom windows | 2.05 m (`X 1.00–3.05`) and 2.00 m (`X 5.60–7.60`) | rear wall | ⚠️ MEASURED |
| Right-flank stair windows | 3 small openings ≈ 0.41 m each at `Y 5.30–5.71`, `6.51–6.90`, `7.70–8.11` | in the wall `X 8.15–8.30` | ⚠️ MEASURED |

---

## 5. Second floor (penthouse) and roof

| Item | Value | Source |
|---|---|---|
| Penthouse room | **6.30 × 4.90** internal | ✅ dimensioned |
| Position | `X 0.14–6.44`, `Y 4.26–9.15` | ⚠️ MEASURED |
| Front glazing | 5.06 m wide (`X 1.14 → 6.20`), facing the front roof terrace | ⚠️ MEASURED |
| Rear window | 3.30 m wide (`X 0.40 → 3.70`) | ⚠️ MEASURED |
| Right-hand glazed wall | 3.64 m long (`Y 4.76 → 8.40`), facing the 1.55 m side terrace | ⚠️ MEASURED |
| Side terrace between penthouse and stair | **1.55 m** | ✅ dimensioned |
| Roof access | via the right-flank stair, arriving at `Y 8.40–8.91` | ⚠️ MEASURED |
| Roof material, drainage, parapet height, penthouse roof form | **not drawn anywhere** | ❓ unknown |

---

## 6. Flagged ambiguities — resolve with the author before drawing conclusions

1. ❓ **Right-flank stair strip (`X 8.30 → 9.10`).** From the first floor upward, a second
   0.80 m wide flight of ~15 treads is drawn **outside** the ground-floor wall line, in the
   1.57 m right side yard. Nothing is drawn there on the ground-floor plan. Two readings:
   (a) the stair core widens above ground and cantilevers 0.80 m over the side setback;
   (b) it is a drafting overlap of the up/down flights. Because the strip has three small
   windows in the wall at `X 8.15–8.30` facing it, reading (a) is the more literal one.
   *Not used as a feature in the visualisation prompts.*
2. ❓ **Rear 1.30 m strip (`Y −1.30 → 0`).** Drawn as a hollow band across the full 8.30 m
   width on the first-floor and roof plans; absent on the ground-floor plan. Reads as a
   rear balcony / service slab at first-floor level. Not visible from the street.
3. ❓ **Front glazing width conflict** — 4.25 m (ground) vs 3.65 m (first) vs one flush
   panel on the elevation. See §4.1.
4. ❓ **Balcony frame width** — plan `4.95 m` starting at `X 4.65`; the elevation draws the
   frame `4.75 m` starting at `X 5.05` (a 0.20/0.40 m discrepancy, ≈ 4 %).
5. ❓ **Bar glazed door width** — plan 1.80 m; elevation 1.65 m.
6. ❓ **Penthouse front glazing width** — plan 5.06 m; elevation draws a 4.20 m two-pane window.
7. ❓ **No height dimension exists on any sheet.** All Z values in §7 are derived from the
   elevation via a scale that was itself derived. See §7 for why they are trustworthy to
   roughly ±3 %.
8. ❓ **No section, no north point, no site orientation, no material schedule, no window
   schedule, no level datum, no room labels on the living room or kitchen.**

---

## 7. Front elevation (`Facade.pdf`) — composition and derived heights

The elevation sheet carries **no dimension lines whatsoever**. A scale was derived and then
cross-checked; it holds to better than 1 % on four independent horizontal features:

| Feature | Elevation, at 46.198 pt/m | Plan | Match |
|---|---|---|---|
| Left mass overall width | 5.05 m | 5.05 m | exact |
| Left stone reveal | 0.40 m | 0.40 m column | exact |
| Main glazed panel | 4.25 m (`X 0.40 → 4.65`) | 4.25 m (`X 0.40 → 4.65`) | exact |
| Entrance portal (travertine surround) | 1.50 m | 1.50 m structural opening | exact |
| Entrance door leaf | 1.20 m | 1.20 m leaf | exact |

Because five independent horizontal features land exactly, the **vertical** readings below
are taken as reliable — but every one of them is still ⚠️ **MEASURED**, never dimensioned.

### 7.1 Derived heights (Z, from ground-floor FFL)

| Level | Z | Note |
|---|---|---|
| Front garden grade | **−1.00 m** | the house sits on a 1.00 m plinth; the entrance platform is at FFL |
| Ground floor FFL | 0.00 | |
| Underside (soffit) of the cantilevered balcony frame | **+2.98 m** | |
| First floor FFL / balcony floor | **+3.78 m** | ⇒ ground storey ≈ 3.78 m floor-to-floor |
| Head of the double-height glazing | **+6.76 m** | |
| Head of the balcony opening | **+6.76 m** | aligns exactly with the glazing head |
| Roof slab / top of the two-storey mass | **+7.36 m** | ⇒ first storey ≈ 3.58 m |
| Top of the balcony frame (parapet upstand) | **+7.96 m** | 0.60 m proud of the main roof line |
| Penthouse window sill | **+7.36 m** | sits on the roof slab |
| Penthouse window head | **+10.36 m** | 3.00 m tall |
| Top of penthouse parapet | **+11.16 m** | |
| **Total height above front grade** | **+12.16 m** | |

### 7.2 Bay-by-bay composition of the front facade (left → right)

**Bay A — the double-height glazed panel.** `X 0.40 → 4.65`, `Z 0.00 → 6.76`.
A **4 columns × 3 rows** grid of glass, 12 panes. Pane widths ⚠️ 0.94 / 1.00 / 1.00 / 1.01 m;
row heights ⚠️ 2.20 / 2.16 / 2.20 m; mullions and transoms ⚠️ 0.10 m wide. Framed on all
four sides by a stone band: 0.40 m at each jamb, 0.60 m over the head to the roof line, and
a 1.00 m plinth below the sill down to garden grade. Drawn with a dense black stipple
hatch = the dark stone cladding.

**Bay B — the cantilevered balcony volume.** `X 5.05 → 9.80` on the elevation
(plan: `4.65 → 9.60`), `Z 2.98 → 7.96`. Drawn as a deep **picture frame** with splayed
reveals on all four sides, in a coarser mid-grey stipple — a different, lighter stone than
Bay A. Frame band 0.40 m on the sides, 0.80 m below the balcony floor, 1.20 m above the
opening head. The opening itself is `X 5.45 → 9.40` × `Z 3.78 → 6.76` (≈ 3.95 × 2.98 m).
Within the opening, left to right:
- a dark reveal, then the **1.65 m two-leaf glazed door** to the Bar (`X 5.75 → 7.40`);
- a **dark recessed panel** `X 7.60 → 8.30` — the balcony's return wall in shadow;
- an **open void** `X 8.30 → 9.40` where the balcony oversails the ground-floor wall line
  and there is nothing behind it but sky.
**The frame's right-hand 1.50 m has no building under it — it cantilevers over the parking
court.** This is the single strongest move in the composition.

**Bay C — the entrance, under the cantilever.** `X 5.05 → 6.55`, `Z 0.00 → 2.98`.
A **1.50 m wide light-stone portal** (drawn in a fine white/pale stipple, i.e. a pale stone,
against the black of everything around it), containing a **1.20 m × 2.50 m single door leaf**
with a **horizontal pull bar at Z ≈ +1.10 m**. The door is drawn in a warm red-brown with
fine vertical grain lines = a timber leaf.

**Bay D — the dark right-hand panel.** `X 6.55 → 8.30`, `Z 0.00 → 2.98`. A flat black
recessed plane, marked with a diagonal, forming the side of the entrance recess.
Beyond `X 8.30` at ground level there is **nothing** — open forecourt.

**Bay E — the setback penthouse.** `X 0.00 → 6.60`, `Z 7.36 → 11.16`.
A second, thinner **picture frame** in solid black: a 0.40 m outer band, then a **0.80 m
pale reveal**, then a **4.20 m × 3.00 m two-pane window** (`X 1.20 → 5.40`, mullion at
`X 3.25–3.35`, panes 2.05 m each). Because it is set back 3.20 m, it reads as a **floating
dark box above and behind the main mass**, stopping 1.70 m short of the right edge.

### 7.3 What the elevation shows about materials (as drawn, colour-coded)

| Element | As drawn | Reading |
|---|---|---|
| Bay A frame, plinth, and the flanks | dense black stipple | dark stone, large panels |
| Bay B balcony frame | coarser mid-grey stipple, splayed reveals | a second, lighter stone; deep reveal |
| Entrance portal | fine white / pale stipple | pale stone surround |
| Entrance door | warm red-brown, vertical grain, horizontal bar handle | timber leaf, long bar handle |
| Glazing | cyan gradient, white frames, 0.10 m mullions | clear glass, slim mullions |
| Bay D, balcony recess | flat black | shadowed recess |
| Bay E frame | solid black + pale reveal | dark frame, pale reveal |

---

## 8. One-line summary

A 3-level, 8.30 × 12.50 m urban villa on a ≈ 256 m² plot: a dark stone two-storey block
whose left bay is a single 4.25 × 6.76 m double-height window; a lighter stone
picture-frame balcony (4.95 × 1.80 m) cantilevering 1.50 m sideways over the parking court
with the entrance tucked beneath it in a 1.50 m pale-stone portal; and a 6.30 × 4.90 m
penthouse set back 3.20 m behind a roof terrace. The house stands on a 1.00 m plinth
looking down a 9.08 m front garden holding a 3.50 × 5.50 m pool on the left and a 3.65 m
two-car forecourt on the right.
