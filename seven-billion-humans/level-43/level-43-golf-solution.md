
## Idea

Manually add the numbers together

* Get values 1-9
* Move down and add 1-9 to the above row


size
* 10 / 11
success
* 25 / 25
speed
* 62s / 53s

```
-- 7 Billion Humans (2214M) --
-- 43: Multiplication Table --

a:
step n
if c != nothing or
 s != datacube:
	jump a
endif
mem1 = set n
b:
step s
mem2 = calc n + mem1
pickup c
write mem2
drop
jump b



```
