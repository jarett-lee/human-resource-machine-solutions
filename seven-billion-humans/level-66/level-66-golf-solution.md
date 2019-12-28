
## Runs
size
* 23 /23
success
* 25 / 25
speed
* 311s / 120s

## Code
```
-- 7 Billion Humans (2214M) --
-- 66: Decimal Counter --

step s
if s == button:
	a:
	listenfor hi
	step s
	step n
	jump a
endif
step s
comment 0
b:
mem1 = calc e + 0
mem2 = set 0
if c != 9:
	mem2 = calc c + 1
endif
c:
if e == mem1 and
 se != button:
	jump c
endif
if mem1 == 9 and
 e == 0 or
 se == button:
	pickup c
	write mem2
endif
pickup n
drop
if mem1 != 9 or
 e != 0 and
 se != button or
 w != worker:
	tell everyone hi
endif
if se == button:
	listenfor hi
endif
jump b


DEFINE COMMENT 0
eJxjYBgFo2AUjGQAAAQEAAE;



```
