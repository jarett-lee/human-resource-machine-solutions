
## Idea

* Move one left
* Die if you're not against the left wall or if you have the same value as the one below you
* Sort yourself

This exploits the game's randomness generator. There are 9 people on the left
wall and we need every number between 0 and 6 inclusive. The probability of
this happening is the probability of rolling every face of a 7-sided dice at
least once in a sequence of 9 rolls.

* google "probability of rolling every face on a dice"
* find https://math.stackexchange.com/questions/1506930/probability-of-rolling-every-face-of-a-die-at-least-once-in-a-sequence-of-n-thro
* k-faced dice and n throws
* k(k−1)^n − (k_C_2)(k−2)^n + (k_C_3)(k−3)^n - ...
* Use a spreadsheet to calculate it

The probability of this happening is less than 5.8%, but in the 100 attempts
I ran, it never failed, which means there's something not so random about the
distribution of datacube values.

## Runs

size
* 11 / 11
success
* 25 / 25
* 25 / 25
* 25 / 25
speed
* 22s / 75s
* 22s / 75s
* 22s / 75s

```
-- 7 Billion Humans (2214M) --
-- 44: Unique Fashion Party --

pickup s
step w
a:
if w != wall or
 s == myitem:
	mem1 = nearest hole
	step mem1
endif
if n > myitem or
 n == nothing:
	step n
else:
	if myitem > s:
		step s
	endif
endif
jump a



```
