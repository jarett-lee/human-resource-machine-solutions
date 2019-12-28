
# If solution


# Calc solution

## Runs
size
* 37 / 23
success
* 25 / 25
speed
* 120s / 120s

## Code
```
-- 7 Billion Humans (2214M) --
-- 66: Decimal Counter --

step s
if s == button:
	a:
	listenfor ready
	step s
	step n
	jump a
endif
step s
pickup n
drop
tell everyone ready
if se == button:
	b:
	if c == 9:
		if w == 8:
			tell w hi
		else:
			tell everyone hi
		endif
		mem1 = set 0
		jump c
	else:
		mem1 = calc c + 1
		c:
		pickup c
		write mem1
		drop
		tell everyone ready
	endif
	jump b
endif
d:
if c == 9:
	mem1 = set 0
else:
	if c == 8:
		mem1 = set 9
	else:
		mem1 = set 1
	endif
endif
listenfor hi
pickup c
write mem1
drop
jump d



```

