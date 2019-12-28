
size
* 12 / 12
success
* 25 / 25
speed
* 112s / 60s

```
-- 7 Billion Humans (2214M) --
-- 50: Cubical Communication --

mem1 = set sw
a:
if mem1 > 1:
	listenfor hi
	mem1 = calc mem1 - 1
	jump a
endif
b:
takefrom s
giveto se
step w
mem1 = calc mem1 + 1
if mem1 <= 5:
	jump b
endif
tell everyone hi



```