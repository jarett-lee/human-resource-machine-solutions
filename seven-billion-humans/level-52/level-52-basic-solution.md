
size
* 39 / 24
success
* 25 / 25
speed
* 559s / 158s

```
-- 7 Billion Humans (2214M) --
-- 52: The Mode Code --

a:
step w
if s != nothing:
	jump a
endif
mem4 = set se
b:
step ne
step ne
step n
step n
comment 0
c:
if se != datacube or
 nw != datacube:
	if ne == datacube:
		step n,ne,e
	else:
		if nw == datacube:
			step nw,w,n
		else:
			if se == datacube:
				step s,e,se
			else:
				step w,sw,s
			endif
		endif
	endif
else:
	step nw,w,sw,n,s,ne,e,se
endif
if c == 99:
	jump c
endif
comment 1
mem1 = calc 0 + c
pickup c
write 99
drop
step mem4
comment 2
d:
if mem1 > 0:
	mem1 = calc mem1 - 1
	step e
	jump d
endif
pickup c
mem1 = calc myitem + 1
write mem1
drop
step mem4
step nw
jump b


DEFINE COMMENT 0
eJxjYBgFo2AUjGQAAAQEAAE;

DEFINE COMMENT 1
eJxjYBgFo2AUjGQAAAQEAAE;

DEFINE COMMENT 2
eJxjYBgFo2AUjGQAAAQEAAE;


```
