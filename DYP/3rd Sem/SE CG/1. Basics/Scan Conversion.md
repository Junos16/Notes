### Line
- DDA
	`len= max(abs(x2-x1), abs(y2-y1)) 
	`del_x = (x2 - x1) / len`
	`del_y = (y2 - y1) / len`
	`x = x1 + 0.5*sgn(del_x)`
	`y = y1 + 0.5*sgn(del_y)`
	`i = 1`
	`while i <= len:`
		`putpixel(x, y)`
		`x += del_x`
		`y += del_y`
		`i++`
- Bresenham
	- Simple
		`x = x1; y = y1;`
		`del_x = x2 - x1`
		`del_y = y2 - y1`
		`m = del_y/del_x`
		`e = m - 0.5`
		`i = 0`
		`while i <= del_x:`
			`putpixel(x, y)`
			`while e >= 0:`
				`y++; e--`
			`x++; e += m`
			`i++`
	- Integer:
		`e = m - 0.5`
			`e'/2*del_x = del_y/del_x - 0.5`
			`e' = 2*del_y - del_x` 
		`e--  ->  e' -= 2*del_x`
		`e += m  ->  e' += 2*del_y`
	- Generalized:
		`x = x1; y = y1`
		`s1 = sgn(x2 - x1)`
		`s2 = sgn(y2 - y1)`
		`del_x = abs(x2 - x1)`
		`del_y = abs(y2 - y1)`
		`if del_y > del_x:`
			`swap(del_x, del_y)`
			`interchange = 1`
		`else:`
			`interchange = 0`
		`e' = 2*del_y - del_x`
		`i = 0`
		`while i <= del_x:`
			`putpixel(x, y)`
			`while e' >= 0:`
				`if interchange = 1:`
					`x += s1`
				`else:`
					`y += s2`
			`if interchange = 1:`
				`y += s2`
			`else:`
				`x += s1`
			`e' += 2*del_y`
			`i++`

### Circle
- DDA
- Bresenham
- Midpoint

### Antialiasing