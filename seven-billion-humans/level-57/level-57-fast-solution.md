
# forEachDir solution

It's nice that forEachDir happens to not run when a person is picking up a data cube.

## Runs
size
* 22 / 16
success
* 25 / 25
speed
* 96s / 100s

## Code
```
-- 7 Billion Humans (2214M) --
-- 57: Neighborly Sweeper --

if e == wall:
	a:
	step w
	if c == datacube:
		mem1 = set 0
		mem2 = foreachdir nw,w,sw,n,s,ne,e,se:
			if mem2 == datacube:
				mem1 = calc mem1 + 1
			endif
		endfor
		pickup c
		write mem1
		drop
	endif
	jump a
else:
	b:
	step e
	if c == datacube:
		mem1 = set 0
		mem2 = foreachdir nw,w,sw,n,s,ne,e,se:
			if mem2 == datacube:
				mem1 = calc mem1 + 1
			endif
		endfor
		pickup c
		write mem1
		drop
	endif
	jump b
endif



```

# Explicit solution (TODO)

```
-- 7 Billion Humans (2214M) --
-- 57: Neighborly Sweeper --

if e == wall:
	step w
	step w
	if c == datacube:
		pickup c
		if s == datacube:
			if n == datacube:
				write 4
			else:
				write 2
			endif
		else:
			if n == datacube:
				write 3
			endif
		endif
		drop
	endif
	step w
	if c == datacube:
		pickup c
		if se == datacube:
			if nw == datacube:
				write 4
			else:
				write 6
			endif
		else:
			if sw == datacube:
				write 4
			else:
				write 5
			endif
		endif
		drop
	endif
	step w
	if c == datacube:
	endif
else:
	step e
	step e
	if c == datacube:
		pickup c
		if ne == datacube:
			write 1
		else:
			if e == datacube:
				write 2
			else:
				write 1
			endif
		endif
		drop
	endif
	step e
	if c == datacube:
		pickup c
		write 2
		drop
	endif
	step e
	if c == datacube:
		pickup c
		if s == datacube:
			write 4
		else:
			write 2
		endif
		drop
	endif
	step e
	if c == datacube:
		pickup c
		if s == datacube:
			write 5
		else:
			write 4
		endif
		drop
	endif
	step e
	if c == datacube:
		pickup c
		write 4
		drop
	endif
endif



```
