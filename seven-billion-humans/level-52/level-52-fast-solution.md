
## Idea
Each person counts how many there are of a specific number.

## Future
Improve by splitting the group into two and counting the two halves of the square or by writing to every other bottom square.

## Runs

size
* 31 / 24
success
* 25 / 25
speed
* 156s / 27s

## Code

```
-- 7 Billion Humans (2214M) --
-- 52: The Mode Code --

mem4 = nearest datacube
if w == worker:
	pickup mem4
	a:
	if w != datacube:
		jump a
	endif
	mem1 = calc w + 1
	write mem1
	drop
endif
b:
step n
if c != datacube:
	jump b
endif
c:
step w
if w == datacube:
	jump c
endif
d:
e:
if c == mem1:
	mem2 = calc mem2 + 1
endif
if n == datacube:
	step n
	jump e
endif
step e
f:
if c == mem1:
	mem2 = calc mem2 + 1
endif
if s == datacube:
	step s
	jump f
endif
if ne == datacube:
	step e
	jump d
endif
pickup mem4
write mem2
drop



```
