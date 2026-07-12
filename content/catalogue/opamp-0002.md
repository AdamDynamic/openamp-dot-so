+++
title = "Quad LFO"
subtitle = "Four triangle/square LFOs on one Kosmo panel."
number = "OPAMP-0002"
category = "synth-module"
contributor = "Marta"
date = 2025-02-21
skill = "Beginner"
build_time = "Two evenings"
img = "img/module.jpg"
img_alt = "Populated DIY module boards, awaiting their panels"
ink = "#26754A"
summary = "One op-amp integrates, another flips: four gentle LFOs on one panel, and the recommended first board in the catalogue."
plate_note = "Marta’s, mid-build — boards first, panels to follow."
cover = "half"
repo = "https://github.com/open-amplitude/opamp-0002"
provides = ["Schematic", "Board Gerbers", "Panel drilling drawing", "BOM", "Build guide"]
licence = "CC BY-NC-SA 4.0"

note = """
I wanted a module a beginner could finish in a weekend and actually
use every day after. Nothing here bites: no calibration, no matched
parts, no surprises. Build it, plug it in, and let two channels wobble
while two crawl. If it works first time, that was the design, not
luck.
"""

[[purchase]]
route = "Kit"
price = "£40"
note = "Board, panel and all parts."

[[purchase]]
route = "Built"
price = "£95"
note = "Assembled and tested."

[[spec]]
label = "Format"
value = "Kosmo, 20 cm panel"

[[spec]]
label = "Channels"
value = "4, identical"

[[spec]]
label = "Rate"
value = "0.05 Hz – 30 Hz, two ranges"

[[spec]]
label = "Outputs"
value = "Triangle and square per channel"

[[spec]]
label = "Power"
value = "±12 V, approx. 40 mA"

[[revisions]]
version = "v1.0"
date = 2025-02-21
note = "First listed."
+++

A synth never has enough slow modulation, and an LFO is the friendliest
circuit there is: one op-amp integrates, another flips, and between them
you get a triangle and a square for the price of two resistors' worth of
decisions. This module simply does that four times, with a range switch
per channel so two can wobble while two crawl.

It is the recommended first board in the catalogue. Nothing needs
calibrating, nothing bites, and when it works you have four of something.

{{< photo src="img/oscilloscope.jpg" alt="Triangle and square waveforms on an oscilloscope screen" number="02.1" caption="Triangle and square, as promised, on the scope." >}}

The build guide covers the rest, including what to check first if a
channel sulks — it is nearly always the range switch. Contributed as
the Society's second entry, and the first not from Adam's bench, which
was rather the point.
