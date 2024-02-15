Explication des différentes task du Projet 2 Shell I/O Redirections and filters :

- Task 0 : Le but est d'écrire un script dans le fichier 0-hello_world créer afficher le texte Hello, World.
Pour cela, j'utilise emacs (que j'utiliserai pour tous les autres fichiers) afin d'éditer le fichier en écrivant les deux lignes #!/bin/bash (qui sera réutiliser pour tous les fichiers) et la commande echo "Hello, World". A noter que nous n'écrirons les commandes que sur la deuxième ligne des fichiers.
J'écris ensuite la commande chmod u+x 0-hello_world pour donner au propriètaire du fichier la pemission de l'exécuter, que je réutiliserai pour tous les autres fichiers.

- Task 1 : Le but est d'écrire un script dans le fichier 1-confused_smiley créer préalablement pour d'afficher un smiley confus.
Pour cela, j'écris la commande echo '"'"(Ôo)'". Petite exception où je n'ai pas utiliser emacs mais vi pour cette Task car emacs ne permet pas d'écrire Ô.

- Task 2 : Le but est d'écrire un script dans le fichier 2-hellofile créer préalablement pour afficher le contenu du fichier /etc/passwd.
Pour cela, j'écris la commande cat /etc/passwd.

- Task 3 : Le but est d'écrire un script dans le fichier 3-twofiles créer préalablement pour afficher le contenu des fichiers /etc/passwd et /etc/hosts.
Pour cela, j'écris la commande chown cat /etc/passwd /etc/hosts.

- Task 4 : Le but est d'écrire un script dans le fichier 4-lastlines créer préalablement pour afficher les 10 dernières lignes du fichier /etc/passwd.
Pour cela, j'écris la commande tail -n 10 /etc/passwd, l'option -n permet de sélectionner le nombre de ligne à afficher.

- Task 5 : Le but est d'écrire un script dans le fichier 5-firstlines créer préalablement pour afficher les 10 premières lignes du fichier /etc/passwd.
Pour cela, j'écris la commande head -n 10 /etc/passwd.

- Task 6 : Le but est d'écrire un script dans le fichier 6-third_line créer préalablement pour afficher la troisième ligne du fichier iacta.
Pour cela, j'écris la commande head -n 3 iacta | tail -1, la partie head permet de choisir les 3 premières lignes et la partie tail permet de n'afficher que la troisième et pas les précédentes.

- Task 7 : Le but est d'écrire un script dans le fichier 7-file créer préalablement pour ajouter l’autorisation d’exécution au propriétaire, au propriétaire du groupe et aux autres utilisateurs, au fichier hello.
Pour cela, j'écris la commande chmod ugo+x hello.

- Task 8 : Le but est d'écrire un script dans le fichier 8-cwd_state créer préalablement pour ne donner aucune autorisation au propriétaire et au propriétaire du groupe et ajouter l’autorisation d’exécution, de lecture et d'écriture aux autres utilisateurs, au fichier hello.
Pour cela, j'écris la commande chmod 007 hello.

- Task 9 : Le but est d'écrire un script dans le fichier 9-duplicate_last_line créer préalablement pour ajouter l’autorisation d’exécution au propriétaire et au propriétaire du groupe, ainsi que l’autorisation d'écriture et d'exécution aux autres utilisateurs, au fichier hello.
Pour cela, j'écris la commande chmod 753 hello.

- Task 10 : Le but est d'écrire un script dans le fichier 10-no_more_js créer préalablement pour définir le mode du fichier hello de la même manière que le mode d’olleh.
Pour cela, j'écris la commande chmod --reference=olleh hello, l'option --reference permet d’appliquer les permissions d’un fichier à un autre.

- Task 11 : Le but est d'écrire un script dans le fichier 11-directories créer préalablement pour ajouter l’autorisation d’exécution à tous les sous-répertoires du répertoire courant pour le propriétaire, le propriétaire du groupe et tous les autres utilisateurs.
Pour cela, j'écris la commande chmod -R a+X ./, l'option -R permet de modifier les autorisations à l’ensemble de l’arborescence.

- Task 12 : Le but est d'écrire un script dans le fichier 12-newest_files créer préalablement pour créer un répertoire appelé my_dir avec les autorisations 751 dans le répertoire de travail.
Pour cela, j'écris la commande mkdir -m 751 my_dir, l'option -m permet de définir les autorisations 751 au moment de créer le répertoire my_dir en contournant le umask par défaut du système.

- Task 13 : Le but est d'écrire un script dans le fichier 13-unique créer préalablement pour remplacer le propriétaire du groupe par School pour le fichier hello.
Pour cela, j'écris la commande chown :school hello.

- Task 14 : Le but est d'écrire un script dans le fichier 14-findthatword créer préalablement pour remplacer le propriétaire par vincent et le propriétaire du groupe par staff pour tous les fichiers et répertoires du répertoire de travail.
Pour cela, j'écris la commande chown vincent:staff *.

- Task 15 : Le but est d'écrire un script dans le fichier 15-countthatword créer préalablement pour changer le propriétaire et le propriétaire du groupe de _hello en vincent et staff respectivement.
Pour cela, j'écris la commande chown -h vincent:staff _hello, l'option -h permet de changer la propriété du lien symbolique.

- Task 16 : Le but est d'écrire un script dans le fichier 16-whatsnext créer préalablement pour modifier le propriétaire du fichier hello à vincent uniquement s’il appartient à l’utilisateur guillaume.
Pour cela, j'écris la commande chown --from=guillaume vincent hello.

- Task 17 : Le but est d'écrire un script dans le fichier 17-hidethisword créer préalablement pour modifier le propriétaire du fichier hello à vincent uniquement s’il appartient à l’utilisateur guillaume.
Pour cela, j'écris la commande chown --from=guillaume vincent hello.

- Task 18 : Le but est d'écrire un script dans le fichier 18-letteronly créer préalablement pour écrire le nom de l'utilisateur actuel.
Pour cela, j'écris la commande whoami.

- Task 19 : Le but est d'écrire un script dans le fichier 19-AZ créer préalablement pour écrire le nom de tous les groupes dont l'utilisateur actuel fait partie.
Pour cela, j'écris la commande groups.

- Task 20 : Le but est d'écrire un script dans le fichier 20-hiago créer préalablement pour changer le propriétaire du fichier hello à l'utilisateur betty.
Pour cela, j'écris la commande chown betty hello.

- Task 21 : Le but est d'écrire un script dans le fichier 21-reverse créer préalablement pour créer le fichier hello.
Pour cela, j'écris la commande touch hello.

- Task 22 : Le but est d'écrire un script dans le fichier 22-users_and_homes créer préalablement pour donner au propriètaire du fichier hello la pemission de l'exécuter.
Pour cela, j'écris la commande chmod u+x hello.

- Task 23 : Le but est d'écrire un script dans le fichier 23-empty_casks créer préalablement pour ajouter l’autorisation d’exécution au propriétaire et au propriétaire du groupe, ainsi que l’autorisation de lecture aux autres utilisateurs, au fichier hello.
Pour cela, j'écris la commande chmod 754 hello (voir chmod pour plus de détails).

- Task 24 : Le but est d'écrire un script dans le fichier 24-gifs créer préalablement pour ajouter l’autorisation d’exécution au propriétaire, au propriétaire du groupe et aux autres utilisateurs, au fichier hello.
Pour cela, j'écris la commande chmod ugo+x hello.

- Task 25 : Le but est d'écrire un script dans le fichier 25-acrostic créer préalablement pour ne donner aucune autorisation au propriétaire et au propriétaire du groupe et ajouter l’autorisation d’exécution, de lecture et d'écriture aux autres utilisateurs, au fichier hello.
Pour cela, j'écris la commande chmod 007 hello.

- Task 26 : Le but est d'écrire un script dans le fichier 26-the_biggest_fan créer préalablement pour ajouter l’autorisation d’exécution au propriétaire et au propriétaire du groupe, ainsi que l’autorisation d'écriture et d'exécution aux autres utilisateurs, au fichier hello.
Pour cela, j'écris la commande chmod 753 hello.


