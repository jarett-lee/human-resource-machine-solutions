```
-- 7 Billion Humans (2214M) --
-- 42: Important Email Organization --

mem2 = nearest wall
a:
mem4 = nearest datacube
step mem4
if s != shredder and
 c == datacube:
	pickup c
endif
mem3 = calc myitem / 10
mem4 = nearest shredder
step mem4
b:
step w
if c != 0:
	jump b
endif
c:
if c < mem3:
	step e
	jump c
endif
if myitem == something:
	giveto s
endif
step mem2
jump a



```
