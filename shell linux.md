find :
	syntaxe : 
		si on connait le nom du fichier recherché : find -name fichier.txt (cherchera un fichier texte du nom de "fichier")
		si on connait juste l'extension : find -name *.txt (cherchera tous les fichiers avec l'extension .txt)
grep :
	syntaxe :
		grep "texte recherché" fichier.txt (cherchera "texte recherché" dans fichier.txt)
ls : 
	syntaxe :
		ls : liste les fichiers du répertoire actuel 
		ls -a : liste les fichiers du répertoire actuel (y compris ceux qui sont masqués) 
scp :
	syntaxe :
		pour copier un fichier local sur la machine distante : scp fichier_source.txt login_remote@ip_remote:/home/login_remote/fichier_destination.txt
		pour copier un fichier distant sur la machine locale : scp login_remote@ip_remote:/home/lgoin_remote/fichier_distant.txt fichier_local.txt
ps :
	syntaxe :
		ps : affiche les process actuellement lancés sur la machine par l'user qui l'exécute
		ps aux : affiche tous les process actuellement lancés sur la machine par tous les utilisateurs


opérateurs/symboles :

- & : permet d'exécuter une commande en arrière plan (syntaxe : touch fichier.txt & ls)
- && : permet la même chose que & mais tout est exécuté en une seule commande (syntaxe : touch fichier.txt && ls)
- > : permet de récupérer le résultat d'une commande pour la rediriger vers une autre en remplaçant totalement (sans append) (syntaxe : echo salut > fichier.txt)
- >> : permet la même chose que > mais avec l'append, le contenu n'est pas overwrite (syntaxe echo coucou >> fichier.txt)

répertoires communs : 

 - /etc : répertoire utilisé pour stocker des fichiers utilisés par l'OS (exemple : sudoers, passwd)
 - /var : répertoire utilisé pour stocker des fichiers qui sont modifiés ou utilisées par des services ou des applications lancées sur le système (exemple : /var/log, contient les logs des applications lancées)
 - /root : équivalent du répertoire /home pour un utilisateur lambda mais pour l'utilisateur root
 - /tmp : répertoire utilisé pour stocker des données temporaires, une fois l'ordinateur redémarré, le contenu de celui-ci est effacé; utile dans une situation de pentesting car par défaut, tous les utilisateurs peuvent y écrire (souvent utile pour stocker des scripts d'énumération par exemple)

vim :
cheatsheet : https://vim.rtorr.com/


crontabs :
	generator : https://crontab-generator.org/
	edit contrabs -> crontab -e













