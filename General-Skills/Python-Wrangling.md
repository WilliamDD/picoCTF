# Python Wrangling

## Files
``` bash
-rw-r--r-- 1 kali kali 1328 Dec  1 16:30 ende.py
-rw-r--r-- 1 kali kali  140 Dec  1 16:31 flag.txt.en
-rw-r--r-- 1 kali kali   33 Dec  1 16:30 pw.txt
```

``` bash
┌──(kali㉿kali)-[~/Downloads]
└─$ python3 ende.py 
Usage: ende.py (-e/-d) [file]

┌──(kali㉿kali)-[~/Downloads]
└─$ cat pw.txt  
6008014f6008014f6008014f6008014f

┌──(kali㉿kali)-[~/Downloads]
└─$ python3 ende.py -d flag.txt.en
Please enter the password:6008014f6008014f6008014f6008014f
picoCTF{*}

```

