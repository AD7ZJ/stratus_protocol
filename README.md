# Stratus Protocl Breakdown
It annoys me that there is no public data (that I could find?) available on the Appareo stratus protocol. Newer units do support the GDL-90 protocol but I guess that will not be ported to older ones. Anyone with info, feel free to contact me or create a pull request here. 

The Stratus PRX V2 seems to output UDP packets on the following ports:
## Port 41501, usually 219 or 60 bytes long
219 bytes:
```
0000   c2 53 ff 10 d4 31 2e 30 2e 30 2e 34 31 00 00 00
0010   00 00 00 00 00 32 2e 31 2e 30 2e 35 30 34 00 00
0020   00 00 00 00 00 31 2e 30 2e 30 2e 33 35 36 00 00
0030   00 00 00 00 00 32 30 30 30 32 34 00 00 00 00 00
0040   45 03 00 00 39 00 0c 07 90 01 25 0a 06 18 01 00
0050   19 00 17 3c f6 00 35 30 31 30 31 30 2d 30 30 30
0060   30 36 37 52 30 30 35 30 31 30 31 30 2d 30 30 30
0070   30 36 36 52 30 38 35 30 31 30 31 30 2d 30 30 30
0080   30 36 35 52 30 30 31 35 30 35 30 30 2d 30 30 30
0090   30 30 34 52 30 30 64 00 00 00 00 00 00 00 30 11
00a0   da 4d ae 69 44 e3 7f 01 00 00 74 fd 4f 0e 20 05
00b0   00 00 08 32 2e 35 2e 31 00 00 00 00 00 00 00 32
00c0   2e 35 2e 31 00 00 00 00 00 00 00 32 2e 35 2e 31
00d0   00 00 00 00 00 00 00 00 20 53 50
```
60 bytes:
```
0000   c2 53 ff 29 35 01 01 ff 00 bb 08 00 00 58 01 00
0010   00 00 00 00 00 00 00 00 00 00 40 00 14 00 00 e2
0020   00 00 00 61 2f 00 00 23 02 00 00 c6 00 11 7f 33
0030   02 00 01 01 01 38 ff 01 00 00 49 20
```


## Port 41502, usually 124 or 48 bytes long
```
0000   c2 53 04 41 75 60 61 02 00 0e 08 08 0d 04 14 1d
0010   17 00 07 0a 0d 06 2c 3c 1a 00 03 12 0d 04 1e 17
0020   8a 00 0e 15 0d 04 17 14 3d 00 02 16 1c 04 1b 33
0030   e1 00 05 17 0d 04 1a 24 47 00 0d 18 0d 04 22 12
0040   30 00 0f 1b 0d 04 1a 21 f0 00 04 1c 0d 04 1a 16
0050   a9 00 00 1f 04 01 00 08 b5 00 0b 20 0d 06 26 50
0060   fd 00 09 85 10 03 1b 2f 9b 00 0c 86 10 01 00 08
0070   02 00 0a 8a 10 01 00 31 ab 00 a9 83
```
48 bytes:
```
0000   c2 53 04 40 29 99 32 02 00 00 73 d6 10 cf 08 97
0010   9f a2 14 8b 61 09 bd b5 0b 17 00 45 73 17 00 02
0020   00 00 00 04 00 13 00 13 00 73 00 00 00 00 6c d1
```

## Port 41504, always 41 bytes long
```
0000   c2 53 04 42 22 71 92 01 00 dc 67 8d ff fb ff 07
0010   00 01 00 f2 ff 1a ff f3 ff 47 e0 d7 f6 87 0c 56
0020   1c 00 00 09 00 11 00 71 ac
```
## Port 41505, always 12 bytes long
```
0000   8d ad 53 95 f8 23 00 03 00 4a b8 00
```
