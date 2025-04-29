no such for loop in python - for (int i = 0; i < 5; i++) {}

In Python, an iterable is an object capable of returning values one at a time.

for i in range(5):
    print(i)

for i in [1, 2, 3, 4]:
    print(i)

they are the same

for c in 'hello':
    print(c)
prints - h e l l o

for x in ('a', 'b', 'c', 'd'):
    print(x)

prints - a, b, c, d

s = 'hello'

for i, c in enumerate(s):
    print(i, c)

enumerate - creates (index, item) pair from elements of iterable