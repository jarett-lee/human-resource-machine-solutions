I can optimize the both solution for speed by attempting to get the people closer to the bottom hole. I can do this by adding a few explicit south east steps. There's a balance between adding too many south east steps since it takes a small amount of time for a south east step to be skipped if the person is against the wall. I found 6 south east steps gave 19 second runs most reliably.

## Runs

size
* 11 / 11
success
* 25 / 25
speed
* 20s / 75s
* 20s / 75s
* 20s / 75s
* 20s / 75s
* 20s / 75s
* 19s / 75s
* 19s / 75s
* 20s / 75s
* 20s / 75s
* 20s / 75s

```
-- 7 Billion Humans (2214M) --
-- 44: Unique Fashion Party --

pickup s
step w
a:
if w != wall or
 s == myitem:
	step se
	step se
	step se
	step se
	step se
	step se
	mem1 = nearest hole
	step mem1
endif
if n > myitem or
 n == nothing:
	step n
else:
	if myitem > s:
		step s
	endif
endif
jump a



```
