
# Sum solution

## Runs
size
* 37 / 26 
success
* 25 / 25
speed
* 64s / 90s

## Code
```
-- 7 Billion Humans (2214M) --
-- 54: Terrain Leveler --

a:
step n
if c != datacube:
	jump a
endif
b:
mem1 = calc mem1 + c
if n == datacube:
	step n
	jump b
endif
pickup c
write mem1
drop
if e == datacube or
 e == worker:
	step n
	c:
	if sw == datacube:
		step w
		jump c
	endif
	mem1 = set s
	step s
	d:
	step s
	if s == datacube:
		jump d
	endif
	pickup c
	listenfor go
else:
	e:
	step w
	mem1 = calc mem1 + c
	if w == datacube:
		jump e
	endif
	pickup c
	mem1 = calc mem1 / 49
	write mem1
	tell everyone go
endif
f:
write mem1
drop
step e
if c == datacube:
	pickup c
	jump f
endif



```

# Guess solution

## Runs
size
* 
success
* 25 / 25
speed
* 

## Code
```
-- 7 Billion Humans (2214M) --
-- 54: Terrain Leveler --

a:
if c != datacube:
	step n
	jump a
endif
b:
pickup c
write 4
drop
if n == datacube:
	step n
	jump b
endif
c:
pickup c
write 5
drop
if s == datacube:
	jump c
endif
d:
pickup c
write 5
drop
if s == datacube:
	jump d
endif



```
