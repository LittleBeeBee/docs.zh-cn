# bitmap_to_array

## description

### Syntax

```Haskell
 ARRAY<BIGINT> BITMAP_TO_ARRAY (BITMAP)
```

将 BIMTAP 转化为ARRAY<BIGINT>，将一个BIMTAP中的所有值组合成一个ARRAY<BIGINT>

## example

```Plain text
mysql> select bitmap_to_array(bitmap_from_string("1, 7"));
+----------------------------------------------+
| bitmap_to_array(bitmap_from_string('1, 7'))  |
+----------------------------------------------+
| [1,7]                                        |
+----------------------------------------------+

mysql> select bitmap_to_array(NULL);
+-----------------------+
| bitmap_to_array(NULL) |
+-----------------------+
| NULL                  |
+-----------------------+
```

## keyword

BITMAP_TO_ARRAY,BITMAP
