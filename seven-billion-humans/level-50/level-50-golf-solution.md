
size
* 16 / 12
success
* 25 / 25
speed
* 122s / 60s

```
-- 7 Billion Humans (2214M) --
-- 50: Cubical Communication --

a:
if sw == 1:
	tell everyone morning
	listenfor hi
endif
if sw == 2:
	tell everyone ready
	listenfor morning
endif
if sw == 3:
	tell everyone ok
	listenfor ready
endif
if sw == 4:
	tell everyone hi
	listenfor ok
endif
takefrom s
giveto se
step w
jump a



```