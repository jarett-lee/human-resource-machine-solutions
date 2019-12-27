```
-- 7 Billion Humans (2214M) --
-- 42: Important Email Organization --

step e
mem2 = nearest wall
a:
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
