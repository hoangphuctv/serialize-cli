# serialize-cli
serialize, unserialize on cli write by php

php-cli required

Example:



Serialize
```bash
$ echo "['id'=>1]" | serialize
a:1:{s:2:"id";i:1;}
```


Unserialize

```bash
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

```bash
cd /tmp && \
git clone https://github.com/hoangphuctv/serialize-cli.git && \
cd serialize-cli/ && \
chmod +x *serialize && \
sudo cp *serialize /usr/local/bin/ && \
rm -rf /tmp/serialize-cli/
```


### Install without git
```bash
curl https://raw.githubusercontent.com/hoangphuctv/serialize-cli/master/serialize | sudo tee /usr/local/bin/serialize
curl https://raw.githubusercontent.com/hoangphuctv/serialize-cli/master/unserialize | sudo tee /usr/local/bin/unserialize
chmod +x /usr/local/bin/*serialize
```

### Uninstall

```bash
$ sudo rm -f  /usr/local/bin/serialize /usr/local/bin/unserialize
```

