
size
* 18 / 11
success
* 25 / 25
speed
* 265s / 53s

```
-- 7 Billion Humans (2214M) --
-- 20: Reverse Line --

```
-- 7 Billion Humans (2214M) --
-- 43: Multiplication Table --

a:
b:
step n
if n != wall:
	jump b
endif
mem3 = set c
step s
c:
step s
if c > 0 and
 s != nothing:
	jump c
endif
mem2 = set c
d:
step w
if c != nothing:
	jump d
endif
mem1 = calc mem3 x w
step mem2
pickup c
write mem1
drop
jump a



```
