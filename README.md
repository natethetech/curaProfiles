# Cura PRINTER Settings
## Prusa i3 MK2 Original

### START GCODE
<pre>G21 ; set units to millimeters
G90 ; use absolute positioning
M82 ; absolute extrusion mode
M140 S{material_bed_temperature} ; set bed temp
M104 S{material_print_temperature} ; set extruder temp
G28 W ; home all without mesh bed level
M109 S{material_print_temperature} ; wait for extruder temp
G80 ; mesh bed leveling
M190 S{material_bed_temperature} ; wait for bed temp

G92 E0.0 ; reset extruder distance position
G1 Y-3.0 F1000.0 ; go outside print area
G1 X60.0 E9.0 F1000.0 ; intro line
G1 X100.0 E21.5 F1000.0 ; intro line
G92 E0.0 ; reset extruder distance position</pre>

### END GCODE
<pre>M104 S0 ; turn off extruder
M140 S0 ; turn off heatbed
M107 ; turn off fan
G1 X100 Y210; home X axis and push Y forward
M84 ; disable motors</pre>

### Bed Settings
X = <pre>250mm</pre>
Y = <pre>210mm</pre>
Z = <pre>200mm</pre>

Build Plate = <pre>Rectangular</pre>

* Machine center is NOT zero *
* Heated Bed Enable *

### PRINTHEAD SETTINGS
Xmin <pre>31mm</pre>
Ymin <pre>40mm</pre>
Xmax <pre>34mm</pre>
Ymax <pre>31mm</pre>
Gantry <pre>28mm</pre>
Nozzle <pre>0.4 (varies)</pre>
