
## Future
How about coming in from the ends?

# Propagation solution

## Runs

size
* 34 / 7
success
* 25 / 25
speed
* 24s / 27s

## Code
```
-- 7 Billion Humans (2214M) --
-- 51: Identify Yourselves --

step s
pickup c
if w == worker:
	if e == worker:
		listenfor go
		if nw == worker:
			mem1 = calc nw + 3
		else:
			if n == worker:
				mem1 = calc n + 2
			else:
				mem1 = calc ne + 1
				tell ne coffeetime
			endif
			write mem1
			drop
			end
		endif
	else:
		listenfor go
		mem1 = calc nw + 3
		write mem1
		drop
		end
	endif
	write mem1
else:
	write 1
endif
step ne
step e
tell se go
tell s go
tell sw go
listenfor coffeetime
step w
step sw
drop



```

# Explicit solution

## Runs

size
* 35 / 7
success
* 25 / 25
speed
* 4s / 27s

## Code

```
-- 7 Billion Humans (2214M) --
-- 51: Identify Yourselves --

pickup s
if w != worker or
 e != worker:
	step s
	if nw != worker:
		write 1
	else:
		write 10
	endif
else:
	if w != worker or
	 e != worker:
		step s
		if nw != worker:
			write 2
		else:
			write 9
		endif
	else:
		if w != worker or
		 e != worker:
			step s
			if nw != worker:
				write 3
			else:
				write 8
			endif
		else:
			if w != worker or
			 e != worker:
				step s
				if nw != worker:
					write 4
				else:
					write 7
				endif
			else:
				if w != worker:
					write 5
				else:
					write 6
				endif
				step s
			endif
		endif
	endif
endif
drop



```
