+++
title = "Wasp Filter"
subtitle = "An aggressive 12dB/oct CMOS filter, after the EDP Wasp."
number = "OPAMP-0001"
category = "synth-module"
contributor = "Adam"
date = 2025-02-07
skill = "Intermediate"
build_time = "Two evenings"
featured = true
img = "img/plate-module.jpg"
img_alt = "A black-and-silver DIY modular synthesiser panel with one large knob, on a white background"
plate_note = "The correspondent's own, third panel revision."
ink = "#3057C0"
cover = "half"
repo = "https://github.com/open-amplitude/opamp-0001"
provides = ["Schematic", "Board Gerbers", "Panel drilling drawing", "BOM", "Build guide"]
licence = "CC BY-NC-SA 4.0"
summary = "CMOS inverters run linear, snarling the way no well-behaved filter will — with proper CV inputs and a panel you can find in the dark."

note = """
The first entry had to be a filter, and it had to be this one. The Wasp
was cheap, plastic and slightly wrong, and it made a noise nothing
polite has made since. Kosmo's big panels suit it: one large knob you
can find in the dark, and enough space between the jacks that a patch
doesn't become surgery. Build the board in one sitting and the panel in
another; the second evening is the one you'll enjoy.
"""

[[purchase]]
route = "Kit"
price = "£45"
note = "Board, panel and all parts. You supply the solder and the patience."

[[purchase]]
route = "Built"
price = "£110"
note = "Assembled, calibrated and burnt in."

[[spec]]
label = "Format"
value = "Kosmo, 20 cm panel"

[[spec]]
label = "Core"
value = "4069UBE hex inverter, run linear"

[[spec]]
label = "Slope"
value = "12 dB/oct, low-pass and band-pass"

[[spec]]
label = "Power"
value = "±12 V, approx. 35 mA"

[[spec]]
label = "CV inputs"
value = "Cutoff ×2, resonance ×1"

[[revisions]]
version = "v1.0"
date = 2025-02-07
note = "First listed."

[[revisions]]
version = "v1.1"
date = 2025-05-23
note = "Panel drawing: corrected pot spacing. Schematic unchanged."
+++

The EDP Wasp got its bite from doing something the datasheet tells you not
to do: running CMOS logic inverters as linear amplifiers. They distort
early, they distort asymmetrically, and pushed hard they snarl in a way a
well-behaved OTA filter never will. This module borrows that misbehaviour
for the Kosmo format, with proper CV inputs and enough panel to grab in
the dark.

The build is straightforward but not tiny — count on two evenings, one
for the board and one for the panel wiring. The 4069 must be the
unbuffered part (4069**UB**); the buffered one will oscillate politely
and sound like nothing at all. Everything else is jellybean.

{{< schematic name="wasp-block" number="01.1" caption="Signal path. The 4069 stages do the filtering and, past a point, the damage." >}}

## What you need

- The board and panel — Gerbers and drilling drawing above, or the kit
- 2 × 4069UBE hex inverters, socketed
- 1 × TL074, 1 × dual-gang 100k pot, 2 × 100k pots
- Jacks, knobs and the passives in the BOM
- ±12 V Kosmo power, 10-pin ragged-edge tolerance included
- A drill and a centre punch, if you're making your own panel

## The work

1. Populate the board smallest-first: resistors, sockets, film caps,
   then the electrolytics and headers.
2. Fit the ICs and bring it up on current-limited power if you have it;
   the build guide gives the voltages you should see.
3. Drill the panel from the drawing — centre-punch everything before
   you drill anything.
4. Mount pots and jacks loosely, square them by eye, then tighten.
5. Wire panel to board following the loom diagram; leave slack, you'll
   thank yourself at repair time.
6. Calibrate: one trimmer, set by ear against the build guide's
   reference patch. If it squelches, it's right.

{{< photo src="img/modular.jpg" alt="Patch cables strung across a modular synthesiser case" number="01.2" caption="In the case, mid-patch. The filter earns the sockets nearest your right hand." >}}
