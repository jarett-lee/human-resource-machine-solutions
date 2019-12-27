This solution uses randomness and long if statements.

size
* 10 / 10
success
* 25 / 25
speed
* 155s / 175s

```
-- 7 Billion Humans (2214M) --
-- 58: Good Neighbors --

a:
b:
step nw,w,sw,n,s,ne,e,se
if c != datacube or
 c == 99:
	jump b
endif
pickup c
c:
step nw,w,sw,n,s,ne,e,se
if c != nothing or
 nw == datacube or
 ne == datacube or
 sw == datacube or
 se == datacube or
 s == datacube:
	jump c
endif
write 99
drop
jump a



```
