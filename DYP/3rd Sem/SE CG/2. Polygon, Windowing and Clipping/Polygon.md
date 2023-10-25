
### Types

- Convex
	- Line joining 2 pts in polygon lies completely inside
- Concave
	- Line not necessarily inside
- Complex
	- Intersecting Boundary
### Representation
- Polygon Primitive
- Trapezoid Primitive
- Line and Point
	- OpCode
	- X coord
	- Y coord
### Inside Test
- Even - Odd Test
	- Point =/= Vertex
		- Odd = Inside
		- Even = Outside
	- Point = Vertex
		- Vertex counts as even
			- When two edges of the polygon meeting lie on same side of line
		- Vertex counts as odd
			- When two edges of the polygon lie on opposite sides of line
- Winding Number Test
	- Look at edges of Polygon 
		- Down = 1
		- Up = -1
		- Sum = Winding Number
			- WN = 0 Outside
			- WN =/= 0 Inside
	- Since it looks at edges passing through lines, vertex case is averted
### Polygon Filling Algorithms
- Seed Fill
	- Seed Point -> Neighbour Pixel -> Boundary Pixel
	- Boundary/Edge Fill
		- Start from seed
		- Check if current pixel is boundary or filled
		- Neither -> Recursively apply algo to 8/4 connected pixels
	- Flood-Fill
		- Same recursive algo as boundary
		- Check for old color instead of boundary/filled
		- Replace old with new
- Scan Line
	- Scan Line moves from y_max to y_min
	- For each iteration start from x_min
	- Line segment formed by intersection
		- Inside -> Fill, Outside-> Skip