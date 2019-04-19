# serialize-cli
serialize, unserialize on cli write by php

php-cli required

Example:



Serialize
```
$ echo "['id'=>1]" | serialize
a:1:{s:2:"id";i:1;}
```


Unserialize

```
$ echo "['id'=>1]" | serialize | unserialize 
array (
  'id' => 1,
)
```

```
$ cat data.dat
a:1:{s:2:"id";i:1;}

$ cat data.dat | unserialize 
array (
  'id' => 1,
)

```
