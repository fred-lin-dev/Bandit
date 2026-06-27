# 2026-06-11

je sais que c'est un cesar tout con mais
j'ai commencé par voir si y'avait pas qqch dasn xxd, j'ai essayé avec l'option -o mais ça na pas donner le rendu attendu.
je suis passer à sort après pour voir si y'a pas un truc de substitution. j'ai essayer avec l'option --sort-human-numeric. mais pareil ça ne ma rien donner de concret.

sur la page de l'exercice j'ai vu un lien vers wiki pour rot13 et y'a quasiment directement la reponse.

tr 'A-Za-z' 'N-ZA-Mn-za-m' <<< "Pack My Box With Five Dozen Liquor Jugs"

j'ai donc essayer directement la redirection avec un fichier

tr 'A-Za-z' 'N-ZA-Mn-za-m' < data.txt

# 2026-06-27
just look at wikipedia

tr 'A-Za-z' 'N-ZA-Mn-za-m' < data.txt
