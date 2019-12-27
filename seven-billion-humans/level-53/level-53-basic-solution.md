
size
* 21 / 16
success
* 25 / 25
speed
* 104s / 80s

```
-- 7 Billion Humans (2214M) --
-- 53: 100 Cubes on the Floor --

if ne != wall or
 se != wall:
	mem1 = set 1
endif
a:
if w != datacube:
	step w
	jump a
endif
if mem1 == 1:
	listenfor ok
endif
tell everyone ok
step w
b:
if ne == worker or
 n == worker:
	jump b
endif
mem1 = calc n + 1
if n == wall:
	mem1 = set 0
endif
c:
pickup c
write mem1
drop
step w
mem1 = calc mem1 + 10
if c == 0:
	jump c
endif



```
