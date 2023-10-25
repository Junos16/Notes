### Viewing Transformation
- Window
	- ***Windowing*** - Process of selecting and viewing picture with different views
	- Inside visible
	- Outside clipped
	- Area in world space that is to be projected onto screen 
- Viewport
	- area of display where image appears
	- Described with pixels for screen coordinates
- Transformation:
	- ***World CS*** - coordinates of pictures stored in memory
	- ***Viewing Coords*** - Coords of Window 
	- ***Normalization*** - 
	- ***Physical Device CS*** - mapped coordinates of image on display
	- Steps:
		1. Determine WC from modelling coord transformations
		2. Convert WC to VC
		3. Normalize VC
		4. Convert NVC to PDC