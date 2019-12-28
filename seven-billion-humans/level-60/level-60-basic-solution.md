
# Pair solution

## Runs
size
* 27 / 14
success
* 25 / 25
speed
* 359s / 200s
* 379s / 200s

## Code
```
-- 7 Billion Humans (2214M) --
-- 60: Understaffed Sorting --

mem1 = set w
step s
a:
b:
if w == mem1 and
 w > c:
	pickup c
	giveto w
	pickup w
	tell w hi
endif
if w != mem1 and
 c > e:
	listenfor hi
endif
if myitem == something:
	drop
endif
if e != wall:
	step e
	jump b
endif
step sw
c:
if w != wall:
	step w
	jump c
endif
d:
if n == worker:
	jump d
endif
if mem1 == worker:
	step ne
	listenfor ugh
else:
	step n
	tell e ugh
endif
jump a



```


# Solo solution
This is an initial sort using a single worker.

## Runs
size
* 24 / 12
success
* 25 / 25
speed
* 843s / 200s

## Code
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
