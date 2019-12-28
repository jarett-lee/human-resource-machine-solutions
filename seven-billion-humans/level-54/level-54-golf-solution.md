
# Solution

## Runs
size
* 24 / 16
success
* 25 / 25
speed
* 124s / 90s

## Code
```
-- 7 Billion Humans (2214M) --
-- 54: Terrain Leveler --

a:
step n
mem1 = calc mem1 + c
if n != wall:
	jump a
endif
b:
if e == worker or
 ne == worker or
 se == worker:
	jump b
endif
step s
mem1 = calc mem1 + e
pickup c
write mem1
drop
step s
step n
c:
if nw == worker or
 w == worker or
 sw == worker:
	jump c
endif
mem1 = set w
if w != datacube:
	mem1 = calc c / 49
endif
d:
pickup c
write mem1
drop
step s
if c == datacube:
	jump d
endif



```

# Guess solution
See both solution for details

## Runs
size
* 11 / 26
success
* 25 / 25
speed
* 247s / 90s

## Code
```
-- 7 Billion Humans (2214M) --
-- 54: Terrain Leveler --

a:
b:
pickup c
write mem1
drop
if n != wall:
	step n
	jump b
endif
mem1 = calc mem1 + 1
c:
step s
if s == datacube:
	jump c
endif
jump a



```
