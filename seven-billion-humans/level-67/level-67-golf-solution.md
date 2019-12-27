
Experimentation

doubling
```
  1
  2
  4
  8
 16
 12
  4
  8
 16
```
1. double
2. if > 9, subtract 10

```
  8
 16   1
 32   2 + 1
 64   6
128  12
256   4 + 1
```
1. double
2. if right > 5, add 1
3. if > 9, subtract 10

size
* 25 / 25
success
* 25 / 25
speed
* 271s / 250s

```
-- 7 Billion Humans (2214M) --
-- 67: Decimal Doubler --

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
comment 0
b:
if se == button:
	mem1 = calc 0 + 0
	mem1 = calc 0 + 0
	tell everyone ready
else:
	listenfor ready
endif
mem2 = calc c x 2
if e >= 5:
	mem2 = calc mem2 + 1
endif
if mem2 >= 10:
	mem2 = calc mem2 - 10
endif
if c != mem2:
	pickup c
	write mem2
	drop
endif
jump b


DEFINE COMMENT 0
eJxjYBgFo2AUjGQAAAQEAAE;


```
