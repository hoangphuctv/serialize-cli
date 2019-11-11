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

### Install with git

```
cd /tmp && \
git clone https://github.com/hoangphuctv/serialize-cli.git && \
cd serialize-cli/ && \
chmod +x *serialize && \
sudo cp *serialize /usr/local/bin/ && \
rm -rf /tmp/serialize-cli/
```


### Install without git
```
curl https://raw.githubusercontent.com/hoangphuctv/serialize-cli/master/serialize | sudo tee /usr/local/bin/serialize
curl https://raw.githubusercontent.com/hoangphuctv/serialize-cli/master/unserialize | sudo tee /usr/local/bin/unserialize
```

### uninstall

```
$ sudo rm -f  /usr/local/bin/serialize /usr/local/bin/unserialize
```

