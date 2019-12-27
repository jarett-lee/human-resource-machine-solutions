size
* 25 / 18
success
* 40 / 40
speed
* 208.5s / 200s

```
-- 7 Billion Humans (2214M) --
-- 42: Important Email Organization --

if e != worker:
	step e
	step e
endif
mem2 = nearest wall
a:
step s
step s
mem4 = nearest datacube
step mem4
if s != shredder and
 c == datacube:
	pickup c
else:
	jump b
endif
mem3 = calc myitem / 10
mem4 = nearest shredder
step mem4
c:
if c < mem3:
	step e
else:
	if c > mem3:
		step w
	else:
		giveto s
		b:
		step mem2
		jump a
	endif
endif
jump c



```
