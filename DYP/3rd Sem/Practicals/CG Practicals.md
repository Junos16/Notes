1. Graphics primitives
2. 4 region circle rectangle, arc
3. draw simple object
4. DDA Bresenham Line
5. DDA Line Bresenham Circle
	1. Diamond in circle
	2. incsribed and circumscribed circles in triangle
6. Scan Fill concave polygon
7. 2d transformation
8. Hilbert Curve
	- vars: iteration
	- const:
		- start point (50, 150) (x = 50, y = 150)
		- directions (u = 1, r = 2, d = 3, l = 4)
		- unit length (h = 10)
	- functions:
		- move(dir, len, &x, &y) up = y--
			- lineto(new x, new y)
		- hlibert(d, r, u, l, iter, len, x, y) down ccw
			- i--
			- hil(r, d, l, u) right cw
			- move right
			- hil(d, r, u, l) down ccw
			- move down
			- hil(d, r, u, l) down ccw
			- move left
			- hil(l, u, r, d) left cw
1. Sunrise sunset
2. 