# Pixel Atlas

## Items

```
Tiles = A binary mask of 8x8 pixels

Arrangements = A group of tiles joined together to form a larger sprite
```

## Format

`[AA][BBBBBBBB]...[[C][DD]]...`

```
AA = Number of tiles

[BBBBBBBB] = A tile data, where B represents a full row in binary, ex: "%" = [00100101]

[[C][...]] = An arrangement

C = The size of the arrangement. Ex: 2 is equal to an arrangement of 2x2 tiles. Arrangements are always square.

DD = The id(s) of the tile to load for the arrangement

```

