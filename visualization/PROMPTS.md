# PROMPTS.md — Production prompt set for ChatGPT / GPT Image

Twelve standalone prompts plus the supporting apparatus. Every prompt is **self-contained**:
each one carries the building lock, so you can paste any single prompt into a fresh chat and
get the same building back. Nothing here needs `SPEC.md` or `IDENTITY.md` open alongside it.

---

## 0. How to run this set

**Order.** Run **P01** first. It is the anchor. When you get a frame you're happy with,
**attach that image** to every later prompt and add one line above the prompt:

> *"Same building as the attached image. Keep the massing, the window grid, the stone tones
> and the cantilever exactly as they are. Change only the camera position and the light."*

GPT Image has no seed. The attached anchor image plus the identical building-lock paragraph
is what enforces consistency — do not paraphrase the lock between prompts.

**Aspect ratios.** GPT Image accepts `1024×1024` (1:1), `1536×1024` (3:2 landscape),
`1024×1536` (2:3 portrait). Each prompt below names the one it is written for.

**If a render drifts,** don't re-roll blindly. Re-run the same prompt with one corrective
sentence appended, e.g. *"The balcony frame must overhang past the right-hand ground-floor
wall with open sky visible beneath its outer end."* One correction per attempt.

---

## 1. The building lock

This paragraph is embedded verbatim inside every prompt below. It is reproduced here only so
you can diff it if a prompt gets edited by hand.

> **BUILDING LOCK —** A three-storey contemporary villa, 8.3 m wide, on a 1 m stone plinth.
> The two-storey main block is charcoal honed basalt in large-format panels with fine
> shadow-gap joints. Its left bay is one double-height window, 4.25 m wide and 6.76 m tall,
> a 4-column × 3-row grid of twelve low-iron glass panes in 100 mm bronze-anodised mullions,
> with no floor slab crossing it. To the right, a deep picture-frame volume in pale
> grey-greige honed stone cantilevers 1.8 m forward and 1.5 m sideways over open ground,
> holding a 4.95 × 1.8 m balcony; splayed reveals, warm wood-slat soffit, its head level with
> the head of the big window, its top edge 0.6 m proud of the roof as a parapet upstand.
> Inside it: a 1.8 m two-leaf glazed door, a shadowed return, open sky at the outer end.
> Beneath the cantilever, in shade, the entrance: a 1.5 m warm ivory travertine portal,
> a 1.2 × 2.5 m smoked oak door with a full-height brushed bronze pull bar, micro-cement
> soffit. Above and 3.2 m behind, a setback penthouse floats — a dark frame 6.6 m wide with
> a pale reveal and a 4.2 × 3 m two-pane window — ringed by a roof terrace. Total height
> above grade 12.16 m.

---

## P01 — HERO. Front three-quarter, late afternoon

*The anchor image. Generate this first. `1536×1024`.*

```
Architectural photograph of a contemporary luxury villa, shot from the front-left at a
three-quarter angle, camera at standing eye height 1.6 m, 35 mm lens, verticals perfectly
corrected, no barrel distortion.

BUILDING LOCK — A three-storey contemporary villa, 8.3 m wide, on a 1 m stone plinth. The
two-storey main block is charcoal honed basalt in large-format panels with fine shadow-gap
joints. Its left bay is one double-height window, 4.25 m wide and 6.76 m tall, a 4-column ×
3-row grid of twelve low-iron glass panes in 100 mm bronze-anodised mullions, with no floor
slab crossing it. To the right, a deep picture-frame volume in pale grey-greige honed stone
cantilevers 1.8 m forward and 1.5 m sideways over open ground, holding a 4.95 × 1.8 m
balcony; splayed reveals, warm wood-slat soffit, its head level with the head of the big
window, its top edge 0.6 m proud of the roof as a parapet upstand. Inside it: a 1.8 m
two-leaf glazed door, a shadowed return, open sky at the outer end. Beneath the cantilever,
in shade, the entrance: a 1.5 m warm ivory travertine portal, a 1.2 × 2.5 m smoked oak door
with a full-height brushed bronze pull bar, micro-cement soffit. Above and 3.2 m behind, a
setback penthouse floats — a dark frame 6.6 m wide with a pale reveal and a 4.2 × 3 m
two-pane window — ringed by a roof terrace. Total height above grade 12.16 m.

FOREGROUND: a 9 m deep walled front garden. On the left, a 3.5 × 5.5 m rectangular pool with
dark still water and flush pale stone coping, its long axis running away from the camera
towards the house. On the right, an open two-car forecourt in large pale stone pavers. Three
low steps rise 1 m from the garden to the entrance platform.

LIGHT: late afternoon, sun low and raking from the left, warm 4200 K. Long soft shadows
across the pavers. The stone reads matte and dry, never wet or glossy. The deep cantilever
throws a clean hard shadow over the entrance so the ivory portal glows out of the dark.
Interiors just visible behind the big window, warm 2700 K, restrained.

STYLE: real architectural photography, medium-format digital, f/8, sharp corner to corner,
natural colour, subtle contrast, no HDR halos, no bloom. Clean sky with light high cloud.
Restrained, expensive, quiet. Photorealistic.

DO NOT: no people, no cars, no text, no logos, no watermark, no lens flare, no fisheye, no
tilted horizon, no converging verticals, no balconies other than the one described, no
pitched roof, no columns, no arches, no ornament, no planting on the facade, no visible
downpipes or air-conditioning units, no rendered CGI look, no oversaturated grass.
```

---

## P02 — FACADE PORTRAIT. Dead-on frontal

*The document shot. Proves the bay-by-bay composition. `1024×1536`.*

```
Straight-on architectural photograph of the front facade of a contemporary luxury villa.
Camera exactly perpendicular to the facade, centred on the building, shift-lens perspective,
absolutely parallel verticals and horizontals, 50 mm equivalent, no perspective convergence
whatsoever — an elevation-like photograph.

BUILDING LOCK — A three-storey contemporary villa, 8.3 m wide, on a 1 m stone plinth. The
two-storey main block is charcoal honed basalt in large-format panels with fine shadow-gap
joints. Its left bay is one double-height window, 4.25 m wide and 6.76 m tall, a 4-column ×
3-row grid of twelve low-iron glass panes in 100 mm bronze-anodised mullions, with no floor
slab crossing it. To the right, a deep picture-frame volume in pale grey-greige honed stone
cantilevers 1.8 m forward and 1.5 m sideways over open ground, holding a 4.95 × 1.8 m
balcony; splayed reveals, warm wood-slat soffit, its head level with the head of the big
window, its top edge 0.6 m proud of the roof as a parapet upstand. Inside it: a 1.8 m
two-leaf glazed door, a shadowed return, open sky at the outer end. Beneath the cantilever,
in shade, the entrance: a 1.5 m warm ivory travertine portal, a 1.2 × 2.5 m smoked oak door
with a full-height brushed bronze pull bar, micro-cement soffit. Above and 3.2 m behind, a
setback penthouse floats — a dark frame 6.6 m wide with a pale reveal and a 4.2 × 3 m
two-pane window — ringed by a roof terrace. Total height above grade 12.16 m.

COMPOSITION, left to right, and this order is fixed: (1) the tall glazed grid occupying the
left half; (2) the pale stone cantilever frame occupying the right half, sitting higher and
projecting towards the viewer; (3) the small bright travertine entrance portal tucked under
the right of that frame, low and in shadow; (4) the dark recessed panel closing the right
edge at ground level. The penthouse frame sits centred-left above the roofline, clearly
behind the main plane.

LIGHT: soft overcast-bright, high thin cloud, no direct sun, even illumination that lets the
stone texture and the shadow-gap joints read clearly. Neutral 5600 K.

STYLE: architectural documentation photography, tripod, f/11, high detail in both the stone
grain and the glass. Truthful colour. Photorealistic.

DO NOT: no people, no cars, no text, no watermark, no vignetting, no tilt, no wide-angle
distortion, no extra windows, no pitched roof, no decorative detail, no planting on the
building, no CGI sheen.
```

---

## P03 — BLUE HOUR HERO. Pool reflection

*The money shot for a cover. `1536×1024`.*

```
Architectural photograph of a contemporary luxury villa at blue hour, shot from the far end
of the garden across the pool, camera low at 1.1 m, 28 mm lens, verticals corrected.

BUILDING LOCK — A three-storey contemporary villa, 8.3 m wide, on a 1 m stone plinth. The
two-storey main block is charcoal honed basalt in large-format panels with fine shadow-gap
joints. Its left bay is one double-height window, 4.25 m wide and 6.76 m tall, a 4-column ×
3-row grid of twelve low-iron glass panes in 100 mm bronze-anodised mullions, with no floor
slab crossing it. To the right, a deep picture-frame volume in pale grey-greige honed stone
cantilevers 1.8 m forward and 1.5 m sideways over open ground, holding a 4.95 × 1.8 m
balcony; splayed reveals, warm wood-slat soffit, its head level with the head of the big
window, its top edge 0.6 m proud of the roof as a parapet upstand. Inside it: a 1.8 m
two-leaf glazed door, a shadowed return, open sky at the outer end. Beneath the cantilever,
in shade, the entrance: a 1.5 m warm ivory travertine portal, a 1.2 × 2.5 m smoked oak door
with a full-height brushed bronze pull bar, micro-cement soffit. Above and 3.2 m behind, a
setback penthouse floats — a dark frame 6.6 m wide with a pale reveal and a 4.2 × 3 m
two-pane window — ringed by a roof terrace. Total height above grade 12.16 m.

FOREGROUND: the 3.5 × 5.5 m pool fills the lower third of the frame, water perfectly still,
mirror-flat, no ripples, no jets. The full height of the glazed bay and the underlit
cantilever reflect in it. Flush pale stone coping, no fence, no ladder, no pool furniture.

LIGHT: fifteen minutes after sunset. Deep even cobalt sky, no sun, no stars. The
double-height window is the light source of the picture — warm 2700 K interior light pouring
out across three storeys, the mullion grid crisp against it. Concealed warm linear light
washes the wood-slat soffit under the cantilever and the ivory travertine of the entrance
portal. Two small grazing lights on the stone. Everything else falls to near-black.

STYLE: long-exposure architectural photography, tripod, f/8, 4 seconds, clean shadows, no
noise, no light bloom, no flare, no light trails. Photorealistic, cinematic but restrained.

DO NOT: no people, no cars, no text, no watermark, no pool lights inside the water, no
coloured LEDs, no torch flames, no candles, no visible light fittings, no fog, no rain, no
purple sky, no HDR, no CGI glow.
```

---

## P04 — ENTRANCE. Under the cantilever

*Detail shot. Sells the material palette. `1024×1536`.*

```
Architectural detail photograph of the entrance of a contemporary luxury villa, shot from
2.5 m away at 1.5 m height, slightly off-axis to the left so the depth of the recess reads,
50 mm lens, verticals corrected.

BUILDING LOCK — A three-storey contemporary villa. The main block is charcoal honed basalt
in large-format panels with fine shadow-gap joints. A deep picture-frame volume in pale
grey-greige honed stone cantilevers 1.8 m forward overhead, carrying a balcony above; its
underside is a warm wood-slat soffit. Directly beneath it, in permanent shade, the entrance:
a 1.5 m wide portal of warm ivory travertine, honed, subtle horizontal veining, running full
height as a clean frame; inside it a 1.2 m wide by 2.5 m tall smoked oak door, vertical
grain, flush-fitted, with a full-height brushed bronze pull bar. To the right of the portal,
a flat dark recessed plane in the same charcoal basalt. The floor is a 1 m high stone
platform in large pale stone pavers, reached by three low steps.

SUBJECT: the collision of three materials — warm ivory travertine, smoked oak, charcoal
basalt — plus brushed bronze and the wood-slat ceiling above. The shadow gaps between the
basalt panels must be visible as fine dark lines. The travertine should read pale and warm
against the near-black stone.

LIGHT: soft indirect daylight bouncing off the pale paving into the recess, plus a
concealed warm linear light grazing down the travertine reveal. No direct sun on the door.
Gentle falloff into the depth of the porch. Colour temperature mixed, 4000 K.

STYLE: architectural detail photography, medium format, f/5.6, shallow but controlled depth
of field, tack sharp on the door and handle, exquisite material texture, natural colour, no
HDR. Photorealistic.

DO NOT: no people, no text, no signage, no house numbers, no doorbell panel, no letterbox,
no doormat, no plants, no pots, no furniture, no reflections of a photographer, no lens
flare, no ornament, no panelled or glazed door, no handle other than the vertical bronze bar.
```

---

## P05 — THE CANTILEVER. Worm's-eye study

*Explains the structural idea in one image. `1024×1536`.*

```
Dramatic low-angle architectural photograph of the cantilevered balcony volume of a
contemporary luxury villa, camera at ground level 12 m out and to the right, looking up at
the underside and outer end of the projection, 24 mm lens, verticals deliberately kept
straight, no fisheye.

BUILDING LOCK — A deep picture-frame volume in pale grey-greige honed stone projects 1.8 m
forward from the face of a charcoal honed basalt building and 1.5 m sideways past the
building's ground-floor wall, so its outer end floats over open paving with nothing beneath
it. The frame is a true frame: splayed reveals on all four sides, a stone band 0.4 m at the
sides, 0.8 m under the balcony floor, 1.2 m above the opening. The soffit is warm wood
slats running front to back. It holds a 4.95 × 1.8 m balcony with a frameless low-iron glass
balustrade set back inside the frame. Inside the opening, left to right: a 1.8 m two-leaf
glazed door in bronze-anodised slim mullions, a shadowed return wall, then open sky at the
outer end. Its top edge rises 0.6 m above the main roofline as a clean parapet upstand. To
the left in the frame, the head of a large double-height window with a bronze mullion grid.

SUBJECT: the overhang. The picture must make it obvious that the right-hand end of the frame
carries no building beneath it — sky visible straight through under the outer end.

LIGHT: mid-morning, sun high and behind the building so the soffit is in shade and lit by
bounce off the pale paving. Strong graphic contrast between the pale stone frame, the black
basalt behind it, and the bright sky. 5200 K.

STYLE: architectural photography, f/9, sharp, natural colour, strong geometry, negative
space, no HDR. Photorealistic.

DO NOT: no people, no cars, no text, no watermark, no visible structural props, columns,
brackets or posts under the cantilever, no railings other than the frameless glass, no
planting, no furniture on the balcony, no lens flare, no distortion, no CGI look.
```

---

## P06 — GARDEN AND POOL. House as backdrop

*Landscape context. `1536×1024`.*

```
Architectural landscape photograph of the front garden of a contemporary luxury villa, shot
from the street boundary looking straight up the garden at the house, camera at 1.6 m,
35 mm lens, verticals corrected.

BUILDING LOCK — A three-storey contemporary villa, 8.3 m wide, on a 1 m stone plinth. The
two-storey main block is charcoal honed basalt in large-format panels with fine shadow-gap
joints. Its left bay is one double-height window, 4.25 m wide and 6.76 m tall, a 4-column ×
3-row grid of twelve low-iron glass panes in 100 mm bronze-anodised mullions. To the right,
a deep picture-frame volume in pale grey-greige honed stone cantilevers 1.8 m forward and
1.5 m sideways over the paving, holding a balcony with a warm wood-slat soffit. Beneath it,
a 1.5 m warm ivory travertine portal with a smoked oak door. Above and set back, a dark
penthouse frame with a pale reveal and a two-pane window, ringed by a roof terrace.

GARDEN, and this layout is fixed: the garden is 9 m deep and about 11 m wide, enclosed by a
plain rendered boundary wall in a warm off-white. On the LEFT, a 3.5 × 5.5 m rectangular
pool, dark still water, flush pale stone coping, its long axis pointing at the house, with a
2 m paved strip between the pool head and the facade. On the RIGHT, an open two-car forecourt
in large pale stone pavers, no roof over it, no garage door. Between them, three low steps
1.55 m wide rising to the entrance platform. Planting is minimal and disciplined: a narrow
band of clipped low grasses along the boundary wall, one multi-stem olive tree in the
right-hand corner, nothing else.

LIGHT: early evening, warm low sun grazing the boundary wall from the left, the house partly
in its own shadow, water dark and still. 4000 K.

STYLE: architectural and landscape photography, f/11, deep focus, natural colour, calm,
expensive restraint. Photorealistic.

DO NOT: no people, no cars, no text, no watermark, no lawn furniture, no umbrellas, no
loungers, no pool toys, no fence around the pool, no flowers, no lawn ornaments, no gravel
mounds, no palm trees, no lens flare, no HDR, no CGI grass.
```

---

## P07 — ROOF TERRACE AND PENTHOUSE

*The third level, which no other shot explains. `1536×1024`.*

```
Architectural photograph taken on the roof terrace of a contemporary luxury villa, camera at
1.6 m standing on the terrace near the front parapet, looking back at the setback penthouse,
35 mm lens, verticals corrected.

BUILDING LOCK — The roof terrace sits at the top of a two-storey charcoal honed basalt
block. A setback penthouse room, 6.3 × 4.9 m, stands on it, pulled 3.2 m back from the front
parapet and 1.55 m in from the right-hand edge, so terrace wraps it on three sides. The
penthouse is a dark frame 6.6 m wide with a pale reveal inside it and a large two-pane
window 4.2 m wide and 3 m tall facing the terrace; its right-hand wall is fully glazed along
3.6 m in bronze-anodised slim mullions. The terrace floor is large-format pale stone pavers
on pedestals with open joints. A solid parapet 1.1 m high runs the perimeter in the same
charcoal basalt, capped flush. At the front-right the terrace steps forward and out over the
balcony below.

CONTENT ON THE TERRACE: nothing but the architecture and one low linear bench in warm teak
against the parapet. Concealed linear lighting at the base of the parapet.

LIGHT: golden hour, low warm sun raking across the terrace from the left, long shadows from
the parapet across the pavers, the penthouse glass catching a warm reflection of the sky.
4200 K. City rooftops soft and out of focus beyond the parapet.

STYLE: architectural photography, f/8, sharp, natural colour, calm, restrained. Photorealistic.

DO NOT: no people, no text, no watermark, no pergola, no canopy, no umbrella, no outdoor
kitchen, no jacuzzi, no potted plants in quantity, no railings other than the solid parapet,
no satellite dishes, no air-conditioning units, no water tanks, no pitched roof, no lens
flare, no HDR.
```

---

## P08 — INTERIOR. The double-height living room

*What the void means, from inside. `1024×1536`.*

```
Interior architectural photograph of a double-height living room in a contemporary luxury
villa, shot from the back of the room looking towards the fully glazed front wall, camera at
1.5 m, 24 mm lens, verticals perfectly corrected.

BUILDING LOCK — The room is 6.65 m wide and 7.8 m deep. Its front wall is one double-height
window 4.25 m wide and 6.76 m tall: a 4-column by 3-row grid of twelve low-iron glass panes
in 100 mm bronze-anodised slim-sightline mullions, running from the floor to a ceiling
6.76 m above, with no floor slab and no beam crossing it. Above and behind, the first floor
stops 3 m short of the glass, leaving an open void; a slim first-floor gallery edge with a
frameless glass balustrade runs across the upper right of the frame. Walls are smooth warm
white plaster. The floor is large-format pale stone in a running bond. A single wall of
charcoal honed basalt with fine shadow-gap joints runs down the left side. The ceiling is
micro-cement.

BEYOND THE GLASS: the front garden, a rectangular pool with dark still water directly ahead
and to the left, a pale boundary wall, soft daylight.

FURNITURE, restrained: one long low sofa in oatmeal boucle, a travertine coffee table, one
sculptural floor lamp in brushed bronze, a large flat-weave rug in warm grey. Nothing else.

LIGHT: mid-morning, soft indirect daylight flooding in through the tall glass, gentle
gradient up the height of the room, no direct sun patch on the floor, no harsh contrast.
Balanced 5000 K daylight with a hint of 2700 K from a concealed cove.

STYLE: interior architectural photography, medium format, f/8, tripod, high dynamic range
handled naturally so both the interior and the garden outside are correctly exposed, no HDR
halos, natural colour. Photorealistic.

DO NOT: no people, no text, no watermark, no television, no clutter, no bookshelves, no
plants beyond one, no curtains, no blinds, no visible track lighting, no chandelier, no
pattern, no gold, no marble veining excess, no fisheye distortion, no converging verticals.
```

---

## P09 — INTERIOR. The bar, looking out to the balcony

*First-floor life, and it re-states the cantilever from inside. `1536×1024`.*

```
Interior architectural photograph of a small first-floor bar room in a contemporary luxury
villa, shot from the inside corner looking out through the glazed door onto a deep
cantilevered balcony, camera at 1.5 m, 28 mm lens, verticals corrected.

BUILDING LOCK — The room is 3.5 × 3.45 m. Its front wall holds a 1.8 m wide two-leaf glazed
door in bronze-anodised slim mullions, opening onto a balcony 4.95 m wide and 1.8 m deep set
inside a deep stone picture frame. The frame is pale grey-greige honed stone with splayed
reveals; the balcony soffit overhead is warm wood slats running front to back; the balustrade
is frameless low-iron glass set back inside the frame. Beyond the balcony, the outer end of
the frame overhangs open paving, so sky is visible through it. Inside the room: a wall of
charcoal honed basalt with fine shadow-gap joints behind a floating smoked oak bar counter
with a brushed bronze rail, a micro-cement ceiling, pale stone floor.

CONTENT: two low stools in tan leather at the counter, a row of glassware, one bottle. That
is all.

LIGHT: late afternoon, warm low light entering horizontally through the balcony opening and
striking the back basalt wall, the wood-slat soffit glowing warm, the room interior in
comfortable shade. Concealed warm strip under the bar counter. 4000 K outside, 2700 K inside.

STYLE: interior architectural photography, f/6.3, sharp, natural colour, warm but not
orange, no HDR. Photorealistic.

DO NOT: no people, no text, no watermark, no branded bottles or labels, no neon, no TV,
no clutter, no curtains, no plants, no visible downlights, no columns on the balcony,
no railings other than the frameless glass, no distortion.
```

---

## P10 — NIGHT. From the street

*The building as a lantern. `1536×1024`.*

```
Night architectural photograph of a contemporary luxury villa seen from the street, shot
from the front-right at a three-quarter angle, camera at 1.6 m, 35 mm lens, verticals
corrected, long exposure on a tripod.

BUILDING LOCK — A three-storey contemporary villa, 8.3 m wide, on a 1 m stone plinth. The
two-storey main block is charcoal honed basalt in large-format panels with fine shadow-gap
joints. Its left bay is one double-height window, 4.25 m wide and 6.76 m tall, a 4-column ×
3-row grid of twelve low-iron glass panes in 100 mm bronze-anodised mullions, with no floor
slab crossing it. To the right, a deep picture-frame volume in pale grey-greige honed stone
cantilevers 1.8 m forward and 1.5 m sideways over the paving, holding a 4.95 × 1.8 m balcony
with a warm wood-slat soffit and a frameless glass balustrade. Beneath the cantilever, a
1.5 m warm ivory travertine portal with a 1.2 × 2.5 m smoked oak door and a brushed bronze
pull bar. Above and 3.2 m behind, a setback penthouse frame with a pale reveal and a two-pane
window, ringed by a roof terrace.

FOREGROUND: a two-car forecourt in pale stone pavers, empty; the pool further left, dark and
mirror-still, reflecting the lit facade.

LIGHT: full night, sky near black with a faint warm city glow at the horizon. Three light
sources only — the double-height window glowing warm 2700 K across its whole six-metre
height with the mullion grid black against it; a concealed warm wash across the wood-slat
soffit under the cantilever; a soft downlight on the ivory travertine portal so the entrance
reads as the brightest small point in the picture. The penthouse window a dim warm rectangle
floating above. Everything else in shadow.

STYLE: long-exposure architectural photography, tripod, f/8, 8 seconds, clean deep blacks,
no noise, no bloom, no flare, no light trails, no starburst. Natural colour. Photorealistic.

DO NOT: no people, no cars, no text, no watermark, no street lamps in frame, no coloured
lighting, no uplighters in the pool, no fog or haze machine look, no rain, no moon, no stars,
no HDR, no CGI glow.
```

---

## P11 — AERIAL. Massing and roof terrace

*Reads the whole plot in one frame. `1536×1024`.*

```
Aerial architectural photograph of a contemporary luxury villa on its plot, drone at 25 m
altitude and about 30 m out in front of the house, looking down at roughly 35 degrees,
35 mm lens, no fisheye, verticals kept clean.

BUILDING LOCK — A three-storey villa with an 8.3 × 12.5 m footprint on a plot roughly
11 × 23 m. The two-storey main block is charcoal honed basalt in large-format panels. Its
front-left bay is one tall double-height window with a bronze mullion grid. A pale
grey-greige stone picture-frame volume cantilevers 1.8 m forward and 1.5 m sideways from the
front-right, holding a balcony, with the entrance beneath it. On top, a setback penthouse
6.3 × 4.9 m sits 3.2 m back from the front parapet and 1.55 m in from the right edge, so a
roof terrace in pale stone pavers wraps it on three sides and steps forward over the balcony
at the front right. Solid charcoal parapets all round.

PLOT, and this layout is fixed: the house sits at the back of the plot with only about 1 to
1.6 m of side yard on each flank and a 1.5 to 2 m rear yard. In front, a 9 m deep garden
enclosed by a plain warm off-white boundary wall — a 3.5 × 5.5 m rectangular pool on the
LEFT with dark still water and flush pale coping, an open two-car forecourt in pale pavers
on the RIGHT, and three low steps between them up to the entrance platform.

LIGHT: late morning, sun from the upper left, crisp shadows showing the depth of the
cantilever and the setback of the penthouse. 5000 K. Neighbouring rooftops soft and
desaturated at the edges of the frame.

STYLE: real drone photography, f/8, sharp, natural colour, no HDR, no tilt-shift miniature
effect, no oversaturation. Photorealistic.

DO NOT: no people, no cars, no text, no watermark, no pitched roofs on the subject building,
no solar panels, no water tanks, no satellite dishes, no air-conditioning units, no swimming
pool on the roof, no lawn, no CGI look, no map or plan-view flattening.
```

---

## P12 — MATERIAL MACRO. The corner where three materials meet

*Texture plate for the material board. `1024×1024`.*

```
Extreme close-up architectural detail photograph, camera 0.6 m away, 90 mm macro lens,
shallow depth of field, of the junction where three materials meet on a contemporary luxury
villa.

SUBJECT: a vertical corner. On the left, charcoal honed basalt in large-format panels — flat
matte near-black stone with a fine sandy grain, meeting the next panel across a crisp 10 mm
shadow gap that reads as a pure dark line. On the right, warm ivory travertine, honed, with
soft horizontal veining and open pores, forming the reveal of an entrance portal. Turning the
corner into frame from the right edge, the vertical edge of a smoked oak door — deep
grey-brown timber, straight open grain — and part of a brushed bronze pull bar catching a
single soft highlight along its length. Above, out of focus, the underside of a warm
wood-slat ceiling.

LIGHT: soft raking daylight from the upper left, low angle, grazing across the surfaces so
every texture reads — the grain of the basalt, the pores of the travertine, the brushed
directional lines in the bronze. No direct hard sun. Neutral 5000 K with a warm bounce.

STYLE: material photography, medium format, f/4, focus on the travertine-to-basalt joint,
gentle falloff, natural colour, extremely high micro-detail, no HDR, no over-sharpening.
Photorealistic.

DO NOT: no people, no text, no watermark, no fingerprints, no dust, no dirt, no water drops,
no reflections of a photographer or a studio, no polished or glossy finish on any stone, no
marble, no granite speckle, no visible sealant beads, no screws, no CGI plastic sheen.
```

---

## 2. Global negative list

If a model or an interface takes a separate negative field, use this. Otherwise the
`DO NOT` line inside each prompt already carries it.

```
people, figures, silhouettes, cars, text, lettering, signage, house numbers, logos,
watermarks, captions, dimension lines, pitched roof, gable, tiles, shingles, columns,
pilasters, arches, cornices, mouldings, ornament, shutters, window grilles, curtains,
awnings, pergola, canopy, balustrade railings in metal, external staircases on the front
facade, extra balconies, facade planting, climbing plants, window boxes, air-conditioning
units, satellite dishes, water tanks, solar panels, downpipes, cables, street furniture,
street lamps, fences, coloured LED lighting, pool lighting, fog, haze, rain, snow, lens
flare, starburst, bloom, HDR halos, oversaturation, fisheye, barrel distortion, converging
verticals, tilted horizon, motion blur, noise, CGI plastic sheen, video-game render,
illustration, painting, sketch, collage, double exposure
```

---

## 3. Consistency crib — the ten facts that must survive every image

Check every render against this list before you accept it. These are the things that make it
*this* building rather than a generic modern villa.

1. **The left bay is ONE window, three storeys of glass, 4 across by 3 up.** No floor slab
   crosses it. If you can see a spandrel band at first-floor level, reject the image.
2. **The cantilever overhangs sideways.** Its outer end has open sky beneath it, past the
   ground-floor wall. If a column, wall or post has appeared under it, reject.
3. **The cantilever frame is a lighter stone than the main block.** Two stones, not one.
4. **The head of the balcony opening lines up exactly with the head of the big window.**
5. **The cantilever's top edge stands 0.6 m proud of the main roofline.**
6. **The entrance is small, bright and in shadow, under the cantilever, on the right.**
   Ivory travertine portal, single smoked oak leaf, one vertical bronze bar. Never centred,
   never grand, never double-leaf.
7. **The penthouse is set back and reads as floating behind the roofline,** stopping short of
   the right-hand edge. Never flush with the facade.
8. **The house sits on a 1 m plinth** reached by three low steps.
9. **Pool on the left, forecourt on the right.** Never reversed, never a garage door.
10. **Everything is matte.** Honed stone, no polish, no gloss, no wet look.

---

## 4. Deliberate departures from the CAD, and why

The prompts are not a literal transcription of the drawings. Three decisions were taken, and
they are recorded here so the client can overrule them:

| Departure | Drawing says | Prompts say | Why |
|---|---|---|---|
| Front glazing width | 4.25 m at ground, 3.65 m at first floor, one flush panel on the elevation | one flush 4.25 m panel, full height | the elevation is the design intent; a stepped opening would read as a drafting artefact |
| Right-flank stair | a 0.8 m stair strip appears outside the ground-floor wall line from the first floor up | omitted | flagged as ambiguous in SPEC §6.1; it is not visible from any of these camera positions anyway |
| Planting, boundary wall, paving | nothing is drawn — the site plan has a boundary line, a pool rectangle and two car symbols only | a plain off-white boundary wall, pale stone pavers, one olive tree, clipped grasses | the drawings give no landscape design at all; this is the minimum invention needed to make a photograph, and it is deliberately austere so it reads as a backdrop |

Every dimension quoted in every prompt comes from `SPEC.md`. Where `SPEC.md` marks a value
**MEASURED** rather than dimensioned, the prompt still uses it — but the tolerance is
roughly ±3 %, which is far below what any image model resolves.
