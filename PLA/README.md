# Cura PLA Settings

## Quality
Description | Primary | Comments
--- | --- | ---
**Layer Height** | `0.30mm` | -
**Initial Layer Height** | `0.31mm` | *0.30-0.33mm*
**Line Width** | `0.40mm` | -
**Wall Line Width** | `0.40mm` | -
**Top/Bottom Line Width** | `0.40mm` | -
**Infill Line Width** | `0.40mm` | -

## Shell
Description | Primary | Comments
--- | --- | ---
**Wall Thickness** | `1.2mm` | *0.40-1.6mm*
**Outer Wall Wipe** | `0mm` | -
**Top/Bottom Thickness** | `1.2mm` | *0.90-1.80mm*
**Top/Bottom Pattern** | `Lines` | *Concentric*
**Bottom Pattern Initial Layer** | `Lines` | *Concentric*
**Outer Wall Inset** | `0mm` | -
**Alternate Extra Wall** | `Enabled` | *Disable reduces weight & time*
**Fill Gaps Between Walls** | `Everywhere` | -
**Z-Seam Alignment** | `Shortest` | -
**Ignore Small Z-Gaps** | `Disabled` | -

## Infill
Description | Primary | Comments
--- | --- | ---
**InFill Density** | `15%` | -
**Infill Patter** | `Grid` | *Concentric Infill Sucks*
**Infill Line Directions** | `90` or `45,135` | -
**Infill Overlap Percentage** | `10%` | -
**Infill Wipe** | `0.1mm` | -
**Infill Before Walls** | `Enabled` | -
**Expand Into Infill** | `Disabled` | -

## Material
Description | Primary | Comments
--- | --- | ---
**Default Print Temp** | `200ºC` | -
**Printing Temp** | `200ºC` | -
**Initial Layer Temp** | `200ºC` | -
**Initial Print Temp** | `190ºC` | -
**Final Print Temp** | `185ºC` | -
**Build Plate Temp (Both)** | `55ºC` | -
**Diameter** | `1.85mm` | -
**Flow** | `100%` | -
**Enable Retraction** | `Enabled` | -
**Retract At Layer Change** | `Enabled` | -
**Retraction Distance** | `1.50mm` | -
**Retraction Speed** | `10mm/sec` | *Up to 25mm/sec for firmer filaments, 10 for softer!*
**Retraction Extra Prime** | `None` | -
**Retraction Min Travel** | `10mm` | -
**Max Retraction Count** | `3 (Three)` | -
**Minimum Extrusion Distance Window** | `1.5mm` | -

## Speed
Description | Primary | Comments
--- | --- | ---
**Print Speed** | `45mm/sec` | -
**InFill Speed** | `45mm/sec` | *Other items default-calculated from this setting except those below*
**Outer Wall Speed** | `calculated` | *Match inner wall speed for faster slightly-rougher prints*
**Travel Speed** | `150mm/sec` | *Faster travel has consistently shown me to clean up stringy-drooly*
**Initial Layer Travel** | `150mm/sec` | *See note for Travel speed*
**Num Slower Layers** | `3 (Three)` | *Two for faster prints on sturdier bases*
**Equalize Flow** | `Disabled` | *CAN help with models with lots of bridging, off otherwise*
**Enable Accel Control** | `Disabled` | *CAN speed up print by enabling, but quality will suffer*
**Enable Jerk Control** | `Disabled` | *Enable to either speed up printing (quality suffers) or smooth jerk for tall objects*

## Travel
Description | Primary | Comments
--- | --- | ---
**Combing Mode** | `Off` | *The ALL setting can reduce stringing across walls but slows prints down, NO SKIN is a good compromise*
**Retract Before Outer Wall** | `Enabled` | *Reduces stringing*
**Avoid Printed Parts While Traveling** | `Enabled` | *Disable to reduce print time, but risk getting globbies on the print!*
**Z-Hop When Retracted** | `Enabled` | *Also useful for timelapses, note the z-hop height you set (used in the octoprint trigger)*
**Z-Hop Height** | `1mm` | *Arbitrary over a couple hundred nm*
