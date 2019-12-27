
size
* 20 / 10
success
* 25 / 25
speed
* 6s / 55s

```
-- 7 Billion Humans (2214M) --
-- 13: Injection Sites 2 --

step s
pickup c
step se
step se
if c == nothing:
	drop
endif
step sw
if e != worker:
	step se
	step se
	step se
	step e
	drop
else:
	step sw
endif
if c == nothing:
	drop
endif
step se
step se
step se
step se
drop



```
