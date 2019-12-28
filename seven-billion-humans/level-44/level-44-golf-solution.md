
# Randomness solution

This solution relies heavily on randomness to work, but is quite reliable and quite fast. It's reliable since the random steps are weighted to avoid a person walking to a hole randomly. I believe it can only fail if there's a long sequence of movements south and east or if the final pair of people somehow detect each other.

## Runs

size
* 6 / 11
success
* 25 / 25
* 25 / 25
* 25 / 25
* 25 / 25
speed
* 125s / 75s
* 120s / 75s
* 112s / 75s
* 130s / 75s

## Code

```
-- 7 Billion Humans (2214M) --
-- 44: Unique Fashion Party --

pickup s
a:
step nw,w,sw,n,s,ne,e
if w == myitem or
 n == myitem:
	mem1 = nearest hole
	step mem1
endif
jump a



```

# Randomness solution (reliable with exploit)

This solution relies heavily on randomness to work, but is perfectly reliable by using the exploit. The only way it can fail is if it times out. It takes 2 more command and takes more time, but it can't fail.

## Runs

size
* 8 / 11
success
* 25 / 25
* 25 / 25
* 25 / 25
* 25 / 25
* 25 / 25
speed
* 190s / 75s
* 186s / 75s
* 165s / 75s
* 148s / 75s
* 171 / 75s

## Code
```
-- 7 Billion Humans (2214M) --
-- 44: Unique Fashion Party --

pickup s
step w
a:
step w,n,s
if w == myitem or
 n == myitem or
 nw == myitem or
 sw == myitem:
	step se
	mem1 = nearest hole
	step mem1
endif
jump a



```
