
## Runs

size
* 15 / 16
success
* 25 / 25
speed
* 99s / 80s


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
	listenfor ok
endif
step w
mem1 = calc n + 1
b:
pickup c
write mem1
tell se ok
drop
step w
mem1 = calc mem1 + 10
if c == 0:
	jump b
endif



```
