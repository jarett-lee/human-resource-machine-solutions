
size
* 13 / 9
success
* 25 / 25
speed
* 214s / 50s

```
-- 7 Billion Humans (2214M) --
-- 68: Goodbye, Humans! --

a:
if w == wall and
 e == wall and
 s == hole or
 s == nothing:
	step s
endif
if e == nothing and
 ne != worker:
	step e
else:
	if s == hole and
	 nw != worker and
	 ne != worker and
	 w != worker and
	 e != worker and
	 sw == wall and
	 se == wall and
	 s != worker:
		mem1 = foreachdir nw,w,sw,n,s,ne,e,se:
			tell everyone hi
		endfor
		if nw != worker and
		 n != worker and
		 ne != worker:
			tell everyone goodbye
		endif
	endif
	if w == nothing and
	 nw != worker:
		step w
	endif
endif
jump a



```
