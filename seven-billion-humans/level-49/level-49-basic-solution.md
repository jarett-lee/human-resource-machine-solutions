
size
* 13 / 7
success
* 25 / 25
speed
* 26s / 17s

```
-- 7 Billion Humans (2214M) --
-- 49: Double Sided Destruction --

mem1 = nearest shredder
pickup s
a:
if w != worker:
	giveto mem1
	tell everyone ready
	end
endif
listenfor ready
if e != worker:
	giveto mem1
	tell everyone ready
	end
endif
listenfor ready
jump a



```
