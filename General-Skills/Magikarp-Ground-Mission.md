# Magikarp Ground Mission

## Description
```
Do you know how to move between directories and read files in the shell? Start the container, `ssh` to it, and then `ls` once connected to begin. Login via `ssh` as `ctf-player` with the password, `481e7b14`
```

``` bash
$ ssh ctf-player@venus.picoctf.net -p 54268
```

``` bash
$ cat 1of3.flag.txt 
picoCTF{xxsh_

$ cat instructions-to-2of3.txt 
Next, go to the root of all things, more succinctly `/`

cd /

ls

$ cat 2of3.flag.txt 
0ut_0f_\/\/4t3r_

$ cat instructions-to-3of3.txt 
Lastly, ctf-player, go home... more succinctly `~`

cd ~
$ ls

$ cat 3of3.flag.txt 
1118a9a4}
```

