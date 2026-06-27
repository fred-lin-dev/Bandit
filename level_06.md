# 2025-10-23

I go back to the step4 to try the cmd file:

bandit4@bandit:~$ l
inhere/
bandit4@bandit:~$ cd inhere/
bandit4@bandit:~/inhere$ l
-file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09
bandit4@bandit:~/inhere$ file ./-file00
./-file00: data
bandit4@bandit:~/inhere$ file ./-file07
./-file07: ASCII text
bandit4@bandit:~/inhere$ file --apple ./-file07
./-file07: UNKNUNKN
bandit4@bandit:~/inhere$ file -b ./-file07
ASCII text
bandit4@bandit:~/inhere$ file -b ./-file00
data
bandit4@bandit:~/inhere$ file -c ./-file00
cont	offset	type	opcode	mask	value	desc
bandit4@bandit:~/inhere$ file -f ./-file00
d%\212h\235U\373\247N?CN\207qy\351\030\200\237\312\366\370\240B\211\007\206g4V\207<\010: cannot open `d%\212h\235U\373\247N?CN\207qy\351\030\200\237\312\366\370\240B\211\007\206g4V\207<\010' (No such file or directory)
bandit4@bandit:~/inhere$ file -f ./-file07
<password>: cannot open `<password>' (No such file or directory)
bandit4@bandit:~/inhere$ file ./-file07
./-file07: ASCII text
bandit4@bandit:~/inhere$ cat ./-file07
<password>
bandit4@bandit:~/inhere$ file -f ./-file07
<password>: cannot open `<password>' (No such file or directory)
bandit4@bandit:~/inhere$ exit
logout
Connection to bandit.labs.overthewire.org closed.

for this step I just read the man page of 'find' cmd

find -readable -perm -u=wr -size 1033c

find -size 1033c
also seems to work but didn't check the readablility for the user neither the perms to know if it's not executable

cat ./maybehere07/.file2

# 2026-06-27

cd inhere/

I try:
file maybehere*/*

file maybehere*/* | grep 1033

stat ./*/* | grep -c "1033"
stat ./*/.* | grep -c "1033"
to find all hidden files

I open grep man page
stat ./*/.* | grep -B 5 "1033"

il fallait juste faire
stat ./*/.* | grep -B 1 "1033"

cat ./maybehere07/.file2
