
This solution uses some randomness, but it is pretty reliable.

## Runs
size
* 35 / 11
success
* 25 / 25
speed
* 232s / 250s

## Code
```
-- 7 Billion Humans (2214M) --
-- 61: Lazy Pathways --

step w
step w
a:
b:
if c == 99:
	c:
	mem1 = calc c - 1
	mem2 = foreachdir nw,w,sw,n,s,ne,e,se:
		if mem2 == datacube and
		 mem2 < mem1:
			mem1 = set mem2
		endif
	endfor
	if mem1 < 90:
		mem1 = calc mem1 + 1
		pickup c
		write mem1
		drop
	else:
		jump b
	endif
endif
mem2 = foreachdir nw,w,sw,n,s,ne,e,se:
	if mem2 == 99:
		step mem2
		jump d
	endif
endfor
if nw == wall and
 s == wall:
	step ne
	step ne
	step ne
	step ne
	step ne
else:
	if sw == wall and
	 n == wall:
		step se
		step se
		step se
		step se
		step se
	else:
		step nw,w,sw,n,s
	endif
endif
jump c
d:
jump a



```
