This solution relies heavily on randomness in order to get the matching items next to each other.

size
* 28 / 11
success
* 20 / 20
* 20 / 20
speed
* 365s / 75s
* 341s / 75s

```
-- 7 Billion Humans (2214M) --
-- 44: Unique Fashion Party --

pickup s
mem2 = nearest hole
a:
mem1 = set 0
b:
if n == nothing:
	step n
endif
if w == nothing:
	step w
endif
if w > myitem:
	step w
endif
if n > myitem:
	step n
endif
if e < myitem:
	step e
endif
if s < myitem:
	step s
endif
if w == myitem or
 n == myitem:
	step mem2
endif
if mem1 > 10:
	jump c
endif
mem1 = calc mem1 + 1
jump b
c:
step se
step se
step s,se
step s,se
step s,se
step s,se
jump a



```