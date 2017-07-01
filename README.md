#Cura PRINTER Settings
##Prusa i3 MK2 Original

###START GCODE
<code>G21 ; set units to millimeters
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
G92 E0.0 ; reset extruder distance position</code>

###END GCODE
<code>M104 S0 ; turn off extruder
M140 S0 ; turn off heatbed
M107 ; turn off fan
G1 X100 Y210; home X axis and push Y forward
M84 ; disable motors</code>

###Bed Settings
X = <code>250mm</code>
Y = <code>210mm</code>
Z = <code>200mm</code>

Build Plate = <code>Rectangular</code>

*Machine center is NOT zero*
*Heated Bed Enable*

###PRINTHEAD SETTINGS
Xmin <code>31mm</code>
Ymin <code>40mm</code>
Xmax <code>34mm</code>
Ymax <code>31mm</code>
Gantry <code>28mm</code>
Nozzle <code>0.4 (varies)</code>
