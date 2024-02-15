Explication des différentes task du Projet 1 Shell Permissions :

- Task 0 :
Le but est d'écrire un script dans le fichier 0-iam_betty créer préalablement pour changer l'utilisateur actuel à l'utilisateur betty.
Pour cela, j'utilise emacs (que j'utiliserai pour tous les autres fichiers) afin d'éditer le fichier en écrivant les deux lignes #!/bin/bash (qui sera réutiliser pour tous les fichiers) et la commande su betty. A noter que nous n'écrirons les commandes que sur la deuxième ligne des fichiers.
J'écris ensuite la commande chmod u+x 0-iam_betty pour donner au propriètaire du fichier la pemission de l'exécuter, que je réutiliserai pour tous les autres fichiers.

- Task 1 :
Le but est d'écrire un script dans le fichier 1-who_am_i créer préalablement pour écrire le nom de l'utilisateur actuel.
Pour cela, j'écris la commande whoami.

- Task 2 :
Le but est d'écrire un script dans le fichier 2-groups créer préalablement pour écrire le nom de tous les groupes dont l'utilisateur actuel fait partie.
Pour cela, j'écris la commande groups.

- Task 3 :
Le but est d'écrire un script dans le fichier 3-new_owner créer préalablement pour changer le propriétaire du fichier hello à l'utilisateur betty.
Pour cela, j'écris la commande chown betty hello.

- Task 4 :
Le but est d'écrire un script dans le fichier 4-empty créer préalablement pour créer le fichier hello.
Pour cela, j'écris la commande touch hello.

- Task 5 :
Le but est d'écrire un script dans le fichier 5-execute créer préalablement pour donner au propriètaire du fichier hello la pemission de l'exécuter.
Pour cela, j'écris la commande chmod u+x hello.

- Task 6 :
Le but est d'écrire un script dans le fichier 6-multiple_permissions créer préalablement pour ajouter l’autorisation d’exécution au propriétaire et au propriétaire du groupe, ainsi que l’autorisation de lecture aux autres utilisateurs, au fichier hello.
Pour cela, j'écris la commande chmod 754 hello (voir chmod pour plus de détails).

- Task 7 :
Le but est d'écrire un script dans le fichier 7-everybody créer préalablement pour ajouter l’autorisation d’exécution au propriétaire, au propriétaire du groupe et aux autres utilisateurs, au fichier hello.
Pour cela, j'écris la commande chmod ugo+x hello.

- Task 8 :
Le but est d'écrire un script dans le fichier 8-James_Bond créer préalablement pour ne donner aucune autorisation au propriétaire et au propriétaire du groupe et ajouter l’autorisation d’exécution, de lecture et d'écriture aux autres utilisateurs, au fichier hello.
Pour cela, j'écris la commande chmod 007 hello.

- Task 9 :
Le but est d'écrire un script dans le fichier 9-John_Doe créer préalablement pour ajouter l’autorisation d’exécution au propriétaire et au propriétaire du groupe, ainsi que l’autorisation d'écriture et d'exécution aux autres utilisateurs, au fichier hello.
Pour cela, j'écris la commande chmod 753 hello.

- Task 10 :
Le but est d'écrire un script dans le fichier 10-mirror_permissions créer préalablement pour définir le mode du fichier hello de la même manière que le mode d’olleh.
Pour cela, j'écris la commande chmod --reference=olleh hello, l'option --reference permet d’appliquer les permissions d’un fichier à un autre.

- Task 11 :
Le but est d'écrire un script dans le fichier 11-directories_permissions créer préalablement pour ajouter l’autorisation d’exécution à tous les sous-répertoires du répertoire courant pour le propriétaire, le propriétaire du groupe et tous les autres utilisateurs.
Pour cela, j'écris la commande chmod -R a+X ./, l'option -R permet de modifier les autorisations à l’ensemble de l’arborescence.

- Task 12 :
Le but est d'écrire un script dans le fichier 12-directory_permissions créer préalablement pour créer un répertoire appelé my_dir avec les autorisations 751 dans le répertoire de travail.
Pour cela, j'écris la commande mkdir -m 751 my_dir, l'option -m permet de définir les autorisations 751 au moment de créer le répertoire my_dir en contournant le umask par défaut du système.

- Task 13 :
Le but est d'écrire un script dans le fichier 13-change_group créer préalablement pour remplacer le propriétaire du groupe par School pour le fichier hello.
Pour cela, j'écris la commande chown :school hello.

- Task 14 :
Le but est d'écrire un script dans le fichier 14-change_owner_and_group créer préalablement pour remplacer le propriétaire par vincent et le propriétaire du groupe par staff pour tous les fichiers et répertoires du répertoire de travail.
Pour cela, j'écris la commande chown vincent:staff *.

- Task 15 :
Le but est d'écrire un script dans le fichier 15-symbolic_link_permissions créer préalablement pour changer le propriétaire et le propriétaire du groupe de _hello en vincent et staff respectivement.
Pour cela, j'écris la commande chown -h vincent:staff _hello, l'option -h permet de changer la propriété du lien symbolique.

- Task 16 :
Le but est d'écrire un script dans le fichier 16-if_only créer préalablement pour modifier le propriétaire du fichier hello à vincent uniquement s’il appartient à l’utilisateur guillaume.
Pour cela, j'écris la commande chown --from=guillaume vincent hello.
