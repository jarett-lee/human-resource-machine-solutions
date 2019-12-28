# Very random solution
This solution is so bad it times out nearly 50% of the time, but it only uses 11 lines.

## Runs
size
* 11 / 11
success
* 14 / 25
speed
* 1144s / 250s

## Code
```
-- 7 Billion Humans (2214M) --
-- 61: Lazy Pathways --

a:
step nw,w,sw,n,s,ne,e,se
mem1 = calc c - 1
mem3 = set mem1
mem2 = foreachdir nw,w,sw,n,s,ne,e,se:
	if mem2 < mem3:
		mem3 = set mem2
	endif
endfor
mem3 = calc mem3 + 1
pickup c
write mem3
drop
jump a



```


