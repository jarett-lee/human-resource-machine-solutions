
## Future
How about coming in from the ends or using explicit sets?

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