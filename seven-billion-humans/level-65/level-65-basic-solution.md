
Idea
1. Move to top left
2. Move like text (from left-to-right, top-to-down, going all the way to the left after going down)
3. Find a blank space
4. Move like text
5. Find a datacube
6. Move the datacube to the blank space

Considerations
* Multiple humans will notice the same blank space

Mitigations
* Issue: Multiple humans will notice the same blank space
  * Idea: Keep track of how many blank spaces there are?
  * Idea: Make sure they always go in order?
    * Idea: Reverse text order
      * Issue: going from left-most to right-most will be an issue
        * Idea: Reverse text order and text order

Idea
1. Move to top left
2. Move like text (from left-to-right, top-to-down, going all the way to the left after going down)
3. Find a blank space
4. Move like text
5. Find and pick up a datacube
6. Move reverse like text
7. Move like text
8. Drop in a blank space
9. Go to (1)

Idea
1. Move reverse like text
2. Move like text (from left-to-right, top-to-down, going all the way to the left after going down)
3. Find a blank space
4. Move like text
5. Find and pick up a datacube
6. Move reverse like text
7. Move like text
8. Drop in a blank space
9. Go to (1)

size
* 31 / 25
success
* 25 / 25
speed
* 1378s / 500s


```
-- 7 Billion Humans (2214M) --
-- 65: Defrag Ordered --

mem1 = set 0
comment 2
f:
e:
g:
if w != hole:
	step w
else:
	step ne
	h:
	if e != hole:
		step e
		jump h
	endif
endif
if mem1 == 1 and
 w == hole and
 n == hole:
	mem1 = set 2
	jump b
endif
if mem1 == 2 and
 w == hole and
 n == hole:
	mem1 = set 0
	jump a
endif
jump g
comment 1
a:
b:
c:
if e != hole:
	step e
else:
	step sw
	d:
	if w != hole:
		step w
		jump d
	endif
endif
if mem1 == 0 and
 c == nothing:
	mem1 = set 1
endif
if mem1 == 1 and
 c == datacube:
	pickup c
	jump e
endif
if mem1 == 2 and
 c == nothing:
	drop
	jump f
endif
jump c


DEFINE COMMENT 1
eJztj8FKQlEURdeHSAMDkajXSxJChEKEgsxRQgSJElQKiTUwncSmgYSjcCThoFGEH9HAgQOReJ/RoEGf
0H5+RrhhcQ/33n3OPmWsJCnSpBSwoazZIyBPyDGhTsioQYYGga5Iq8aaquaChM8EdZJ+D+M2NMlxbecl
BdUpLO96lNQxbU7VMrecqcm5+1X954aaqdClzCMlnjiizyEDFRlwwJB9hsozcqZX7fKmjNniXTsmy0Q5
Jp74sZy1ydiMvMcL2zw7VV+he1paZ2bfzJ45RVMhokWkexbqsaDD1PWUNp/cmVhd5nrgy/kjp/w2P94v
5peVVvon+gMLu01e;

DEFINE COMMENT 2
eJztjs1KAmEYhZ8rkWFw4UIkwlXMhcwMpoyWaIsGokVIyCEiYRIF24gLiXDlYojoWroez7juEubA4Tu8
3/P+XAH64EcvfCNK+pTqOcd26pxyJONTI3bc2mO2yvwO2Jvbm/mimpFwoGJ7/Jr5O9emSDlzPTLTKxMt
GGptakWsN7vwliWplvTtB+cn3s0WzM/9GzoUdNx3wTOXmtH1DV0Nnce0dEdITsA9DefANwb+C7mmSULL
m9quRboholatWv/qBEhwPY4;


```



