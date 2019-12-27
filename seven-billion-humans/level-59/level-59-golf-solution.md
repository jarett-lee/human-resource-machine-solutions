
size
* 7 / 7
success
* 25 / 25
speed
* 60s / 15s

```
-- 7 Billion Humans (2214M) --
-- 59: Glory Hole --

a:
mem1 = foreachdir nw,w,sw,n,s,ne,e,se:
	if c > mem1 or
	 c == nothing and
	 mem1 == datacube:
		step mem1
	endif
endfor
if c == 1:
	mem1 = nearest hole
	step mem1
endif
jump a



```

