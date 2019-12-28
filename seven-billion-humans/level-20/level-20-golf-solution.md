
## brainstorm

* pick up = 1
* drop = 1
* move left = 1
* move right = 1
* move down = 1
* jump = 1

already 6 cost

## idea

snake around

* Pick them all up
* Move left
* Move down
* Move right

size
* 9 / 9
success
* 25 / 25
speed
* 11s / 11s

```
-- 7 Billion Humans (2214M) --
-- 20: Reverse Line --

pickup s
a:
if sw == hole:
	step s
	b:
	if e == datacube or
	 e == hole:
		drop
	endif
	step e
	jump b
endif
step w
jump a



```
