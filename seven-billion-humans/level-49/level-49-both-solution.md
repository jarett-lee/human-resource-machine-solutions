
This solution uses unreliable-looking distance and pathing to get the order right.

## Runs

size
* 6 / 7
success
* 25 / 25
speed
* 14s / 17s

## Code

```
-- 7 Billion Humans (2214M) --
-- 49: Double Sided Destruction --

mem1 = nearest shredder
pickup s
a:
if w == worker and
 e == worker:
	jump a
endif
giveto mem1
step sw



```
