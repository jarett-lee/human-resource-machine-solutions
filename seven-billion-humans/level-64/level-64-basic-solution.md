This solution uses signals to have the people move sequentially.

size
* 47
success
* 25 / 25
speed
* 210s / 54s

```
-- 7 Billion Humans (2214M) --
-- 64: Binary Counter --

if s != datacube:
	step s
	step n
	step s
	a:
	tell everyone morning
	listenfor go
	step s
	step n
	jump a
endif
if e != worker:
	step s
	pickup c
	b:
	listenfor morning
	if myitem == something:
		step s
		drop
	else:
		step n
		pickup s
	endif
	tell nw hi
	tell w hi
	tell sw hi
	jump b
endif
step s
pickup c
c:
listenfor hi
if myitem == something:
	if mem1 == 1 and
	 e == worker:
		step s
		drop
	endif
	mem1 = set 0
	if se == datacube:
		mem1 = set 1
	endif
else:
	if mem1 == 1 and
	 ne == worker:
		step n
		pickup s
	endif
	mem1 = set 0
	if e == datacube:
		mem1 = set 1
	endif
endif
tell nw hi
tell w hi
tell sw hi
if nw != worker and
 w != worker and
 sw != worker:
	tell everyone go
endif
jump c
step s



```
