
## Future
Reuse pick up, write, drop code from top of program.

## Runs

size
* 24 / 24
success
* 25 / 25
speed
* 212s / 158s

## Code

```
-- 7 Billion Humans (2214M) --
-- 52: The Mode Code --

mem4 = nearest datacube
pickup mem4
mem3 = nearest datacube
if w == worker:
	a:
	if w == worker:
		jump a
	endif
	mem1 = calc w + 1
	write mem1
endif
drop
step mem3
b:
c:
step w
if w == datacube:
	jump c
endif
d:
if c == mem4:
	mem2 = calc mem2 + 1
endif
if e == datacube:
	step e
	jump d
endif
if n == datacube:
	step n
	jump b
endif
pickup mem4
write mem2
drop



```
