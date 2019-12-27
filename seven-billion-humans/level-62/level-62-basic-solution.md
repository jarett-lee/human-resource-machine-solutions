
size
* 51 / 48
success
* 25 / 25
* 25 / 25
speed
* 122s / 174s
* 124s / 174s

```
-- 7 Billion Humans (2214M) --
-- 62: The Sorting Floor --

step n
step n
step n
step n
step n
a:
if w == hole or
 e == hole:
	listenfor ready
	if myitem == something:
		drop
	endif
	listenfor go
	if myitem == something:
		drop
	endif
	listenfor morning
	if myitem == something:
		drop
	endif
	listenfor hi
	if myitem == something:
		drop
	endif
else:
	if w > c:
		pickup c
		giveto w
		pickup w
		drop
	endif
	tell everyone ready
	if c > e:
		pickup c
		giveto e
		pickup e
		drop
	endif
	tell everyone go
	if w > c:
		pickup c
		giveto w
		pickup w
		drop
	endif
	tell everyone morning
	if e > sw:
		pickup sw
		giveto e
		pickup e
		step sw
		drop
		step ne
	endif
	tell everyone hi
endif
if s != datacube:
	step n
	step n
else:
	step s
endif
jump a



```
