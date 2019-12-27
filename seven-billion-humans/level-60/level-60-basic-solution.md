This is an initial sort using a single worker.

size
* 23 / 12
success
* 20 / 25
speed
* 845s / 200s

```
-- 7 Billion Humans (2214M) --
-- 60: Understaffed Sorting --

step ne
step ne
if n != nothing:
	end
endif
step sw
step sw
a:
pickup s
if se == wall:
	step s
	drop
	step nw
endif
if myitem > se:
	drop
	pickup se
	step s
	drop
	pickup n
	step ne
else:
	step s
	drop
	step nw
endif
jump a



```
