This is an initial sort using a single worker.

size
* 60 / 12
success
* 25 / 25
* 25 / 25
* 25 / 25
* 25 / 25
* 25 / 25
speed
* 163s / 200s
* 156s / 200s
* 156s / 200s
* 160s / 200s
* 161s / 200s

```
-- 7 Billion Humans (2214M) --
-- 60: Understaffed Sorting --

step ne
step ne
if n != nothing:
	end
endif
step se
step se
a:
pickup s
if se == wall:
	step s
	drop
	step nw
else:
	if myitem > se:
		drop
		pickup se
		step s
		drop
		pickup n
		step ne
	else:
		step s
		drop
		step nw
	endif
endif
jump a



```

