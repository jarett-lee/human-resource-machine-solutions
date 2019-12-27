
Idea
1. Put all the datacubes on the sensors
2. Wait for right cube to change (or for button press)
3. If the number to the right goes from 9 to 0
  or there is no number
  1. If the number is 9
    1. Make the number 0
  2. Else
    1. Increment by 1
4. Go to (2)

size
* 26 / 23
success
* 25 / 25
speed
* 249s / 120s

```
-- 7 Billion Humans (2214M) --
-- 66: Decimal Counter --

step s
if s == button:
	a:
	listenfor hi
	step s
	step n
	tell everyone ready
	jump a
endif
step s
pickup n
drop
comment 0
tell everyone hi
b:
if se == button:
	listenfor ready
endif
mem1 = calc e + 0
mem2 = calc c + 1
if mem2 == 10:
	mem2 = set 0
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
	drop
endif
if mem1 != 9 or
 e != 0 and
 se != button or
 w != worker:
	tell everyone hi
endif
jump b


DEFINE COMMENT 0
eJxjYBgFo2AUjGQAAAQEAAE;


```
