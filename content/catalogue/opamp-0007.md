+++
title = "TR-2 Volume Fix"
subtitle = "A quiet rebuild for the Tremolo's lost level."
number = "OPAMP-0007"
category = "pedal-mod"
contributor = "el_farad"
date = 2025-11-14
skill = "Intermediate"
build_time = "An evening"
img = "img/tr2.jpg"
img_alt = "A vintage tremolo pedal"
ink = "#5B9E52"
summary = "Make-up gain where the Tremolo loses it, with a set-once internal trimmer — unity restored for your rig, not the average one."
plate_note = "el_farad’s donor, before the fix went in."
cover = "half"
repo = "https://github.com/open-amplitude/opamp-0007"
provides = ["Schematic", "BOM", "Mod guide"]
licence = "CC BY-NC-SA 4.0"

note = """
Mine came from the classifieds with the volume already gone and a
price to match. The usual advice is to turn something else up, which
moves the problem into somebody else's pedal. Fix it where it breaks.
The trimmer means your unity, on your amp, not the average of
everyone's.
"""

[[purchase]]
route = "Kit"
price = "£11"
note = "Resistors, trimmer and a matched LDR."

[[purchase]]
route = "Pre-modded"
price = "£90"
note = "A donor TR-2, modified, with the trimmer set to unity."

[[spec]]
label = "Fits"
value = "Boss TR-2, all board revisions"

[[spec]]
label = "Fix"
value = "Make-up gain at the output stage, trimmable"

[[spec]]
label = "Trimmer"
value = "Internal; set once, forget"

[[spec]]
label = "Drilling"
value = "None"

[[spec]]
label = "Reversible"
value = "Fully"

[[revisions]]
version = "v1.0"
date = 2025-11-14
note = "First listed."

[[revisions]]
version = "v1.1"
date = 2026-02-27
note = "Guide: added LDR matching note and unity-setting procedure by ear."
+++

Every TR-2 owner learns the same lesson: switch it on and the whole guitar
takes a polite step backwards. The volume drop is baked into the output
stage, and the usual internet answer — turn the level up somewhere else —
just moves the problem along the signal chain.

This fix adds make-up gain where the loss happens, with an internal
trimmer so you can set true unity for your own rig and then close the
box for good. The guide includes a set-by-ear procedure that needs no
meter — match the bypassed level with the effect off, and stop.
