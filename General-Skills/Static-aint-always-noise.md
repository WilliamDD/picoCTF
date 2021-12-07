# Nice netcat

## Description
```
Can you look at the data in this binary: static? This BASH script might help!
```

``` bash
wget https://mercury.picoctf.net/static/ec4dbd8898ade34e1d60d5b70c1b8c8c/ltdis.sh 
wget https://mercury.picoctf.net/static/ec4dbd8898ade34e1d60d5b70c1b8c8c/static
```

``` bash
$ file static 
static: ELF 64-bit LSB shared object, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, for GNU/Linux 3.2.0, BuildID[sha1]=639391a8b15c579d69659462d3c935fa61693f17, not stripped

$ file ltdis.sh 
ltdis.sh: Bourne-Again shell script, ASCII text executable
```

``` bash
$ chmod +x ltdis.sh
```

``` bash
$ ./ltdis.sh static 
Attempting disassembly of static ...
Disassembly successful! Available at: static.ltdis.x86_64.txt
Ripping strings from binary with file offsets...
Any strings found in static have been written to static.ltdis.strings.txt with file offset
```

``` bash
$ cat static.ltdis.strings.txt
1020 picoCTF{*}
```