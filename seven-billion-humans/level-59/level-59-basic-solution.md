
size
* 9 / 7
success
* 25 / 25
speed
* 58s / 15s

```
-- 7 Billion Humans (2214M) --
-- 59: Glory Hole --

mem1 = nearest datacube
step mem1
a:
mem1 = foreachdir nw,w,sw,n,s,ne,e,se:
	if c > mem1:
		step mem1
	endif
endfor
if c == 1:
	mem1 = nearest hole
	step mem1
endif
jump a



```
