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
* X = **250mm**
* Y = **210mm**
* Z = **200mm**
* Build Plate **Rectangular**
* Machine center is **NOT** zero
* Heated Bed **Enable**

### PRINTHEAD SETTINGS
Xmin **31mm**
Ymin **40mm**
Xmax **34mm**
Ymax **31mm**
Gantry **28mm**
Nozzle **0.4 (varies)**
