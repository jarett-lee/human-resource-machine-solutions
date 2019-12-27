A randomness-based solution.

size
* 16 / 11
success
* 25 / 25
speed
* 637s / 250s

```
-- 7 Billion Humans (2214M) --
-- 61: Lazy Pathways --

step w
step w
step w
a:
b:
step nw,w,sw,n,s,ne,e,se
mem1 = calc c - 1
mem3 = set mem1
mem2 = foreachdir nw,w,sw,n,s,ne,e,se:
	if mem2 < mem3:
		mem3 = set mem2
	endif
endfor
if mem3 >= mem1:
	jump b
endif
mem3 = calc mem3 + 1
pickup c
write mem3
drop
jump a



```