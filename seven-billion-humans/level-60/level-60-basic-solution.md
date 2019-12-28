
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
* 18 / 12
success
* 25 / 25
speed
* 694s / 200s

## Code
### Version 3
I believe version 3 is faster compared to version 2 since there's less pick up and drop when going right-to-left.

```
-- 7 Billion Humans (2214M) --
-- 60: Understaffed Sorting --

step ne
step ne
if n == nothing:
	step se
	step se
	a:
	if s > se:
		pickup s
		drop
		pickup se
		step s
		drop
		pickup n
		step e
		drop
		step n
	else:
		step w
	endif
	jump a
endif



```

### Version 2
```
-- 7 Billion Humans (2214M) --
-- 60: Understaffed Sorting --

step ne
step ne
if n == nothing:
	step se
	step se
	a:
	pickup s
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
	jump a
endif



```
