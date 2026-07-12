+++
title = "DS-1 Diode Clipper"
subtitle = "Three clipping voices for the Boss Distortion DS-1."
number = "OPAMP-0004"
category = "pedal-mod"
contributor = "Adam"
date = 2025-06-06
skill = "Beginner to intermediate"
build_time = "An evening"
featured = true
summary = "Silicon, germanium or LED clipping on a rotary switch in the battery bay — reversible, no drilling, an evening at the bench."
img = "img/plate-ds1.jpg"
img_alt = "A well-used orange distortion pedal photographed on a white background"
plate_note = "Jo M.'s, photographed after a year on her board."
ink = "#E8590C"
cover = "feature"
repo = "https://github.com/open-amplitude/opamp-0004"
provides = ["Schematic", "Daughterboard Gerbers", "BOM", "Build guide"]
licence = "CC BY-NC-SA 4.0"

note = """
This started as a repair. A DS-1 came to me with one dead clipper and,
rather than order the same diode again, I tried what was in the drawer.
The germanium pair went in first and stayed for a month. The rotary switch
came later, once it was clear that no single answer suited every amp.
It's the entry I hand to beginners first: the desoldering is honest
practice, and the result earns its place on a board.
"""

[[purchase]]
route = "Kit"
price = "£18"
note = "The daughterboard, all diodes, the rotary switch and hookup wire. You supply the pedal, the iron and the evening."

[[purchase]]
route = "Pre-modded"
price = "£95"
note = "A donor DS-1, modified and tested. Exchange for your own pedal by arrangement."

[[spec]]
label = "Fits"
value = "Boss DS-1, board revisions from 1994 on"

[[spec]]
label = "Clipping voices"
value = "Silicon (stock) / germanium / LED"

[[spec]]
label = "Switching"
value = "3-position rotary, battery compartment"

[[spec]]
label = "Drilling"
value = "None — enclosure stays stock"

[[spec]]
label = "Reversible"
value = "Fully; original diodes retained"

[[spec]]
label = "Current draw"
value = "Unchanged (approx. 4 mA)"

[[revisions]]
version = "v1.0"
date = 2025-06-06
note = "First listed."

[[revisions]]
version = "v1.1"
date = 2025-08-01
note = "BOM: D9E listed as preferred germanium part; 1N34A noted as substitute. Added note on socketing the daughterboard, after Jo M.'s build."

[[revisions]]
version = "v1.2"
date = 2026-01-16
note = "Gerbers: pad spacing enlarged around the rotary switch. Build guide photographs re-shot."
+++

The DS-1 keeps its distortion in one place. After the op-amp gain stage, a
pair of silicon diodes — D4 and D5 — clips the top and bottom off the
signal, and that hard limit, not the transistor boost and not the tone
stack, is most of what you hear as "the DS-1 sound". Change what the diodes
are made of and you change where the clipping starts and how abruptly it
arrives: germanium clips earlier and softer, LEDs later and louder, and the
stock silicon sits in between.

This modification lifts those two diodes onto a small daughterboard
carrying all three pairs, selected by a rotary switch mounted in the
battery compartment — no drilling, and the enclosure stays stock. It is
fully reversible: the original parts are kept, and the pedal can go back to
standard in ten minutes. Expect an evening at the bench, most of it spent
on careful desoldering.

{{< schematic name="diode-clipper" number="04.1" caption="Three clipping voices. The rotary switch selects which pair sits in the signal path to ground." >}}

## What you need

- A Boss DS-1 (any board revision from 1994 on)
- The daughterboard — etch it from the Gerbers, or the kit includes one
- 2 × 1N4148 silicon diodes
- 2 × D9E germanium diodes (1N34A will do; see the BOM for substitutes)
- 2 × 3 mm red LEDs
- A 3-position rotary switch (Lorlin CK series or similar)
- Iron, desoldering braid or pump, side cutters, hookup wire

## The work

1. Open the pedal and photograph the board before touching anything.
2. Desolder D4 and D5. Take your time — the pads lift more easily than
   they should.
3. Solder a wire pair into the vacated pads and route it towards the
   battery compartment.
4. Fit the rotary switch through the daughterboard and mount both against
   the compartment wall with the supplied bracket.
5. Populate the three diode pairs. Match the germanium pair if you can;
   the build guide shows a five-minute method with a multimeter.
6. Test each position before closing up — silicon first, so you know what
   stock sounds like on the way out.

{{< photo src="img/people-solder.jpg" alt="Hands desoldering a small circuit board at a kitchen table, pedal enclosure alongside" number="04.2" caption="Most of the evening is careful desoldering. Take the time it takes." >}}
