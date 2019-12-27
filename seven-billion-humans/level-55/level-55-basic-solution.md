
size
* 8 / 8
success
* 25 / 25
speed
* 24s / 25s

```
-- 7 Billion Humans (2214M) --
-- 55: Data Flowers --

pickup s
a:
step n
if n != datacube or
 s != datacube:
	jump a
endif
mem2 = foreachdir nw,w,sw,n,s,ne,e,se:
	mem1 = calc mem1 + mem2
endfor
write mem1
drop



```
