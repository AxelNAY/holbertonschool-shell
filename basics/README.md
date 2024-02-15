Explication des différentes task du Projet 0 Shell Basics :

- Task 0 :
Le but est d'écrire un script dans le fichier 0-current_working_directory créer préalablement pour afficher le chemin du dossier actuel.
Pour cela, j'utilise emacs (que j'utiliserai pour tous les autres fichiers) afin d'éditer le fichier en écrivant les deux lignes #!/bin/bash (qui sera réutiliser pour tous les fichiers) et la commande pwd pour afficher le chemin. A noter que nous n'écrirons les commandes que sur la deuxième ligne des fichiers.
J'écris ensuite la commande chmod u+x 0-current_working_directory pour donner au propriètaire du fichier de l'exécuter, que je réutiliserai pour tous les autres fichiers.

- Task 1 :
Le but est d'écrire un script dans le fichier 1-listit créer préalablement pour afficher la liste des fichiers et dosssiers du répertoire actuel.
Pour cela, j'écris la commande ls.

- Task 2 :
Le but est d'écrire un script dans le fichier 2-bring_me_home créer préalablement pour revenir dans le home de l'utilisateur.
Pour cela, j'écris la commande cd.

- Task 3 :
Le but est d'écrire un script dans le fichier 3-listfiles créer préalablement pour afficher la liste des fichiers et répertoires du répertoire actuel dans un format long.
Pour cela, j'écris la commande ls -l, l'option -l permet d'afficher les résultats de ls en format long.

- Task 4 :
Le but est d'écrire un script dans le fichier 4-listmorefiles créer préalablement pour afficher la liste des fichiers et répertoires, incluant ceux qui sont cachés, du répertoire actuel dans un format long.
Pour cela, j'écris la commande ls -l -a (ou -la), l'option -a permet d'afficher en plus des résultats de ls -l les fichiers cachés présent dans le répertoire actuel.

- Task 5 :
Le but est d'écrire un script dans le fichier 5-listfilesdigitonly créer préalablement pour afficher la liste des fichiers et répertoires, incluant ceux qui sont cachés, du répertoire actuel dans un format long avec les ID d’utilisateur et de groupe affichés numériquement.
Pour cela, j'écris la commande ls -la -n, l'option -n permet d'afficher les résultats de ls -la avec les ID d’utilisateur et de groupe affichés numériquement.

- Task 6 :
Le but est d'écrire un script dans le fichier 6-firstdirectory créer préalablement pour créer le répertoire my_first_directory dans le répertoire /tmp déjà existant.
Pour cela, j'écris la commande mkdir /tmp/my_first_directory.

- Task 7 :
Le but est d'écrire un script dans le fichier 7-movethatfile créer préalablement pour déplacer le fichier betty (à créer) du répertoire tmp au dossier tmp/my_first_directory.
Pour cela, j'écris la commande mv /tmp/betty /tmp/my_first_directory. /tmp/betty étant le fichier et /tmp/my_first_directory étant la destination.

- Task 8 :
Le but est d'écrire un script dans le fichier 8-firstdelete créer préalablement pour détruire le fichier betty.
Pour cela, j'écris la commande rm /tmp/my_first_directory/betty.

- Task 9 :
Le but est d'écrire un script dans le fichier 9-firstdirdeletion créer préalablement pour détruire le répertoire my_first_directory.
Pour cela, j'écris la commande rmdir /tmp/my_first_directory.

- Task 10 :
Le but est d'écrire un script dans le fichier 10-back créer préalablement pour revenir au répertoire précédent.
Pour cela, j'écris la commande cd -, l'option - permet de revenir au répertoire précédent plutôt que dans le home de l'utilisateur avec un cd simple.

- Task 11 :
Le but est d'écrire un script dans le fichier 11-lists créer préalablement pour lister tous les fichiers, incluant ceux qui sont cachés dans le répertoire courant et le parent du répertoire de travail et du répertoire /boot, au format long.
Pour cela, j'écris la commande ls -la . .. /boot.

- Task 12 :
Le but est d'écrire un script dans le fichier 12-file_type créer préalablement pour écrire le type du fichier iamafile (à créer) du répertoire tmp.
Pour cela, j'écris la commande file /tmp/iamafile.

- Task 13 :
Le but est d'écrire un script dans le fichier 13-symbolic_link créer préalablement pour créer un lien symbolique au fichier bin/ls.
Pour cela, j'écris la commande ln -s /bin/ls __ls__, ln -s permet de créer un lien symbolique (-s pour symbolique), /bin/ls est le fichier cible et __ls__ est le nom du lien.

- Task 14 :
Le but est d'écrire un script dans le fichier 14-copy_html créer préalablement pour copier tous les fichier html dans le répertoire parent.
Pour cela, j'écris la commande cp -u /tmp/test_html/*.html /tmp/, l'option -u permet de ne pas copier de fichiers qui possèdent une modification identique ou plus récente horodatage dans le dossier de destination (tmp).

- Task 15 :
Le but est d'écrire un script dans le fichier 15-lets_move créer préalablement pour déplacer tous les fichiers commençant par une majuscule dans le répertoire /tmp/u.
Pour cela, j'écris la commande mv [[:upper:]]* /tmp/u, l'option [[:upper:]] sélectionne les fichiers commençant par une majuscule.

- Task 16 :
Le but est d'écrire un script dans le fichier 16-clean_emacs créer préalablement pour détruire tous les fichiers se terminant par '~'.   
Pour cela, j'écris la commande find . -name '*~' -delete, find . -name '*~' sélectionne tous les fichiers se terminant par ~ et -delete les détruit.

- Task 17 :
Le but est d'écrire un script dans le fichier 17-tree créer préalablement pour créer les répertoires welcome/, welcome/to/ et welcome/to/school dans le répertoire actuel.
Pour cela, j'écris la commande mkdir -p /tmp/test_tree/welcome/to/school, l'option -p permet de créer des répertoires parents.

