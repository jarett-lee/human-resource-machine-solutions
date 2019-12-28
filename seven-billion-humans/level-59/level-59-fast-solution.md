
# Explicit solution

## Runs
size
* 49 / 7
success
* 25 / 25
speed
* 10s / 15s

## Code
```
-- 7 Billion Humans (2214M) --
-- 59: Glory Hole --

mem1 = nearest datacube
if mem1 > 8:
	if e == wall:
		step sw
	else:
		step se
		if se == 10:
			step se
		endif
	endif
	a:
	if c > 9:
		step s
		jump a
	endif
	step sw
	step w
	step nw
	step nw
	step nw
	step nw
	step w
	step w
	step w
endif
if s == wall:
	step nw
	step nw
	if w != datacube:
		step n
		step n
		step ne
		step n
		step e
	endif
	step nw
	step nw
	step nw
	step n
	step w
endif
if n == wall:
	b:
	if w != hole:
		step w
		jump b
	endif
	c:
	step s
	jump c
endif
step mem1
d:
e:
mem1 = foreachdir ne,e,se:
	if mem1 == datacube and
	 mem1 < c:
		step mem1
		jump e
	endif
endfor
if c == 1:
	mem1 = nearest hole
	step mem1
endif
jump d



```
