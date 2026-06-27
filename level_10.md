# 2026-06-11

j'ai commencé par look les commandes qui pourrais commandes xxd et strings, mais je ne me suis pas attardé et j'ai donc fermé les man. Je suis donc repartit sur la man de grep et j'ai fait:

bandit9@bandit:~$ grep data.txt -e "==="
grep: data.txt: binary file matches
bandit9@bandit:~$ grep data.txt -e "===" -x
bandit9@bandit:~$ grep data.txt -x -e "==="
bandit9@bandit:~$ grep data.txt -xe "==="
bandit9@bandit:~$ echo $?
1
bandit9@bandit:~$ grep data.txt -e "==="
grep: data.txt: binary file matches
bandit9@bandit:~$ echo $?
0
bandit9@bandit:~$ grep data.txt -x "==="
grep: ===: No such file or directory
bandit9@bandit:~$ grep data.txt -e "==="
grep: data.txt: binary file matches
bandit9@bandit:~$ grep -b data.txt -e "==="
grep: data.txt: binary file matches
bandit9@bandit:~$ l

pour au final me rappeler de relire la man de strings car je me suis rappeler que c'est de la gestion de string comme grep.

bandit9@bandit:~$ strings -U data.txt
strings: invalid argument to -U/--unicode: data.txt
bandit9@bandit:~$ strings -d -U data.txt
strings: invalid argument to -U/--unicode: data.txt

et j'ai trouvé le mdp avec la commande:
bandit9@bandit:~$ strings -d data.txt

mais c'est pas optimal, j'ai donc pipe avec grep

strings -d data.txt | grep ===

qui à un meilleur affichage. (ps: on peut aussi changer le nombre de "=" mais il faut que ça soit entre 2 et 10 inclus)


# 2026-06-27
strings -d
me donne déjà la réponse mais avec
strings -d data.txt | grep ===
c'est mieux mais faudrait que je trouve un manière à garder que la partie de droite
