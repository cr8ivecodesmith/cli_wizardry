#### Split a large file

Syntax:

```
split -b [CHUNK_SIZE] [LARGE_FILE] [CHUNK_FILES]
```

Usage:

```
split -b 5m some_large_archive.tar.gz some_large_archive.tar.gz.part-
```


#### Combine the large file again

Syntax:

```
cat [CHUNK_FILES] > [LARGE_FILE]
```

Usage:

```
cat some_large_archive.tar.gz.part-* > some_large_archive.tar.gz
```
