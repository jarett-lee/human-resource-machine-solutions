
size
* 24 / 28
success
* 25 / 25
speed
* 127s / 95s

```
-- 7 Billion Humans (2214M) --
-- 63: Defrag Disordered --

a:
mem1 = nearest datacube
step mem1
step n
step n
step n
step s
pickup mem1
b:
if n != hole:
	step n
	jump b
endif
c:
d:
if w != hole:
	step w
	jump d
endif
e:
if c == nothing:
	drop
	f:
	if s != hole:
		step s
		jump f
	endif
	jump a
endif
if e != hole:
	step e
	jump e
endif
step s
jump c



```
