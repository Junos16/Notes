- Clipping - Division of each element of picture into visible and invisible portions
- Determine inside outside clip window
- Point Clipping
	- ${x_{w}}_{min} \leq x \leq {x_{w}}_{max}$
	- ${y_{w}}_{min} \leq y \leq {y_{w}}_{max}$

### Line Clipping
- Inside (Both endpoints are inside boundary)
- Outside
		- Partially
			- Both endpoints are outside but on either sides of window
			- One endpoint is inside the window
		- Completely
			- Both points are outside but both endpoints lie on the same side of the window
- Cohen-Sutherland Algorithm
	- opcodes:
		- INSIDE = 0
		- LEFT = 1, RIGHT = 2 
		- BOTTOM = 4, TOP = 8
	- Line Cases:
		- op1 & op2 == 0
			- op1 == op2 == 0 -> inside
			- else partially visible
		- op1 & op2 != 0
			- completely outside window
	- While loop:
		- Check visibility of endpoint
		- Clip accordingly
		- Check until the final clipped line is completely visible
	- Midpoint
		- Check visibility and then Divide line
		- check visibility again for each piece and divide line accordingly
		- Keep dividing until the divided lines are either completely visible or invisible

### Polygon Clipping
- Cannot just clip each edge as result isnt necessarily a closed polygon
- Sutherland Hodgeman Algorithm
	- Multiple subroutines to clip each vertex with each edge of the window
	- After each step intermediate polygon is passed to the next step
	- In each stage:
		- Cycle through each vertex
		- v1->out and v2->in, save v1'->inter and v2
		- v1->in and v2->in, save v2
		- v1->in and v2->out, save v1'->inter
		- If v1->out and v2->out, save nothing
- Weiler Atherton Algorithm
	- For concave polygons
	- Initialize:
		- Clip Polygon = Window
		- Subject Polygon = Polygon to be cclipped
	- Loop:
		- Start from an arbitrary vertex on clip polygon and move to next adj vertex
		- If tracing edge enters Clip Polygon
			- Record intersection
			- Continue Tracing
		- If tracing edge leaves Clip Polygon
			- swap Clip Polygon and Subject Polygon
			- Continue tracing
		- If tracing edge forms sub-polygon, then submit that along with result
			- Continue tracing rest of original Subject Polygon from a recorded intersection poijnt that marks beginning of notyet traced portion of edge
		- Loop terminates when the entire border of the original subject polygon has been traced exactly once

### Generalized Clipping
- Generalize to arbitrary convex clipping window
- Similar clipping routines for all each boudary
- Recursion to call each routine using only parameters of specific boundaries

### Interior Exterior Clipping
- Interior -> Regular Clipping
- Exterior -> Remove everything inside clipping widow
- Used when high priority windows overlap with low priority ones