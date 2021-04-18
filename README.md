# Marlin Firmware for my 3D Printer

This contains my customised configuration.h file, specific to my printer.

All other standard files can be downloaded from: https://marlinfw.org/

The changes I made (as seen in the file):

	- Number of extruders and filament diameter
	- Type of thermistors and for which component (hotend, heated bed)
	- Min and max temperatures (safety features)
	- Extrusion min temperature (can only extrude melted filament)
	- Invert endstops (useful for tuning)
	- Stepper motor drivers - I used A4988
	- Axis steps per unit - this is the number of steps (a stepper motor has a certain number of steps per revolution) that corresponds to 1mm of axis motion
	- Max feedrate - how fast an axis can move. I set a low value for the z-axis.
	- (I didn’t use a z probe)
	- Invert the axis/extruder motor directions - useful when tuning, and is easier than flipping the wire connections
	- Set endstops to be either min or max
	- Set the size of heated bed and the travel limits (i.e. maximum print volume)
	- Set constants for preheating, which can activated via the LCD
	- Set LCD and SD card settings (language, type, control direction)

Note - if using an LCD, you may need to install the U8glib library.
