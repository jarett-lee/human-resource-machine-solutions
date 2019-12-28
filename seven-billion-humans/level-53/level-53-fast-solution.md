
## Runs

size
* 35 / 16
success
* 25 / 25
speed
* 70s / 80s


## Code
```
-- 7 Billion Humans (2214M) --
-- 53: 100 Cubes on the Floor --

a:
if w != datacube:
	step w
	jump a
endif
if n != wall:
	if s != wall:
		listenfor ok
		step w
		if s > 0:
			mem1 = calc s - 1
			pickup c
			write mem1
			tell ne ok
		else:
			mem1 = calc n + 1
			pickup c
			write mem1
			tell se ok
		endif
		drop
	else:
		step w
		pickup c
		write 9
		tell ne ok
		mem1 = set 9
		drop
	endif
else:
	step w
	tell se ok
endif
b:
step w
mem1 = calc mem1 + 10
pickup c
write mem1
drop
if w != wall:
	jump b
endif



```
