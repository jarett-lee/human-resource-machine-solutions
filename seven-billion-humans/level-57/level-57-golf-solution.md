
size
* 14 / 16
success
* 25 / 25
speed
* 122s / 100s

```
-- 7 Billion Humans (2214M) --
-- 57: Neighborly Sweeper --

a:
if e != wall:
	if ne != worker and
	 se != worker:
		step e
	endif
	jump a
endif
b:
step w
if c == datacube:
	mem1 = set 0
	mem2 = foreachdir nw,w,sw,n,s,ne,e,se:
		if mem2 == datacube:
			mem1 = calc mem1 + 1
		endif
	endfor
	pickup c
	write mem1
	drop
endif
jump b



```