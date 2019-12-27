
size
* 8 / 8
success
* 25 / 25
speed
* 13s / 14s

```
-- 7 Billion Humans (2214M) --
-- 56: Local Maximums --

step w
step w
mem2 = foreachdir nw,w,sw,n,s,ne,e,se:
	if mem2 > mem1:
		mem1 = set mem2
	endif
endfor
pickup mem1
mem1 = nearest shredder
giveto mem1



```
