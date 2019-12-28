
# Guess solution
The program ends when the average is filled-in, so guessing values from 0 to 10 will eventually give the average. I didn't include 0-1 as guesses since I'm guessing those averages never occur.

## Future
Try more guess attempts

## Attempts
I tried:
* inside out: 5, 6, 4, 7, 3, 8, 2, 9, 1
* inside out: 5, 4, 6, 3, 7, 2, 8, 1, 9
* top to bottom: 
* low to high from 2
  * example: 2, 3, 4, 5, 6, 7, 8, 9, 10
  * size: 19
  * success: 100 / 125
  * results: 87s, 127s, 76s, 101s, 115s

## Runs
size
* 19 / 26
success
* 25 / 25
speed
* 83s
* 96s

## Code
```
-- 7 Billion Humans (2214M) --
-- 54: Terrain Leveler --

mem1 = set 2
a:
if c != datacube:
	step n
	jump a
endif
b:
c:
pickup c
write mem1
drop
if n == datacube:
	step n
	jump c
endif
mem1 = calc mem1 + 1
d:
pickup c
write mem1
drop
if s == datacube:
	step s
	jump d
endif
mem1 = calc mem1 + 1
jump b



```
