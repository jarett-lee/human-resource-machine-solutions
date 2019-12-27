
Idea (cost 11)
1. (cost 1) pick up datacube
2. (cost 3) move to the left wall
3. (cost 2) if there's a gap, drop
3. (cost 3) move to the right wall
4. (cost 1) move down
5. (cost 1) jump to (2)

Experimentation

minimum cost
1 pick up
1 move
1 loop
1 drop

move right if above a datacube? then I don't need to check if I need to check if I need to drop or not

Idea (cost 10)
1. (cost 1) pick up datacube
2. (cost 3) if above a datacube, move right and drop
3. (cost 1) else
3. (cost 3) move to the left wall
4. (cost 1) move down
5. (cost 1) jump to (2)

size
* 10 / 10
success
* 25 / 25
speed
* 165s / 55s

```
-- 7 Billion Humans (2214M) --
-- 13: Injection Sites 2 --

pickup s
a:
if c == datacube and
 e != wall or
 s == wall:
	step e
	drop
else:
	b:
	if w != wall:
		step w
		jump b
	endif
	step s
endif
jump a



```
