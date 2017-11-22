# Project 01

Project 01 implementation as described [here](//nand2tetris.org/01.php).

- NOT Gate

```c++
IN in;
OUT out;
```

```c++
out = not in
```

- AND Gate

```c++
IN a, b;
OUT out;
```

```c++
if a == 1 and b == 1
    out = 1
else
    out = 0
```

- OR Gate

```c++
IN a, b;
OUT out;
```

```c++
if a == 1 or b == 1
    out = 1
else
    out = 0
```

- XOR Gate

```c++
IN a, b;
OUT out;
```

```c++
out = not a == b
```

- Multiplexor

```c++
IN a, b, sel;
OUT out;
```

```c++
if sel == 0
    out = a
else if set == 1
    out = b
```

- Demultiplexor

```c++
IN in, sel;
OUT a, b;
```

```c++
if set == 0
    {a, b} = {in, 0}
else if set == 1
    {a, b} = {0, in}
```

- 16-bit NOT

```c++
IN in[16];
OUT out[16];
```

```c++
for i = 0..15:
    out[i] = not in[i]
```

- 16-bit AND

```c++
IN a[16], b[16];
OUT out[16];
```

```c++
for i = 0..15:
    out[i] = (a[i] and b[i])
```

- 16-bit OR

```c++
IN a[16], b[16];
OUT out[16];
```

```c++
for i = 0..15:
    out[i] = (a[i] or b[i])
```

- 16-bit Multiplexor

```c++
IN a[16], b[16], sel;
OUT out[16];
```

```c++
for i = 0..15:
    if sel == 0
        out[i] = a[i]
    else if sel == 1
        out[i] = b[i]
```

- 8-way OR

```c++
IN in[8];
OUT out;
```

```c++
out = (in[0] or in[1] or ... or in[7])
```

- 4-way 16-bit Multiplexor

```c++
IN a[16], b[16], c[16], d[16], sel[2];
OUT out[16];
```

```c++
if sel == 00
    out = a
else if sel == 01
    out = b
else if sel == 10
    out = c
else if sel == 11
    out = d
```

- 8-way 16-bit Multiplexor

```c++
IN a[16], b[16], c[16], d[16],
   e[16], f[16], g[16], h[16],
   sel[3];
OUT out[16];
```

```c++
if sel == 000
    out = a
else if sel == 001
    out = b

...

else if sel == 111
    out = h
```

- 4-way dDemultiplexor

```c++
IN in, sel[2];
OUT a, b, c, d;
```

```c++
if sel == 00
    {a, b, c, d} = {in, 0, 0, 0}
else if sel == 00
    {a, b, c, d} = {0, in, 0, 0}
else if sel == 00
    {a, b, c, d} = {0, 0, in, 0}
else if sel == 00
    {a, b, c, d} = {0, 0, 0, in}
```

- 8-way Demultiplexor

```c++
IN in[8];
OUT out;
```

```c++
out = (in[0] or in[1] or ... or in[7])
```