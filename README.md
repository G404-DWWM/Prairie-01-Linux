# Prairie-01-Linux
## Atelier Learning By Teaching

### Instructions :	
Vous devez lire les articles et restituer 3 à 5 points que vous jugez importants.  
Timing : Préparer : 30mn  
Restitution : Google Slide ou Google Docs  + Oral (5 minutes)  


**Linux vs Windows vs MacOS**
  - [Différences entre Linux et Windows](https://framablog.org/2008/09/02/differences-entre-linux-et-windows/)
  - [Linux vs Windows](https://www.ionos.fr/digitalguide/serveur/know-how/linux-vs-windows/)
  - [What are the differences between MacOS and Linux](https://qastack.fr/ubuntu/11392/what-are-the-differences-between-mac-os-and-linux)
  - [Wikipedia - MacOS](https://fr.wikipedia.org/wiki/MacOS)
	  
**Distributions Linux / Noyau Linux**
  - [Distribution Linux](https://fr.wikipedia.org/wiki/Distribution_Linux)
  - [Ubuntu - Kernel](https://doc.ubuntu-fr.org/kernel)
 
**Open Source vs Logiciel Libre**
  - [Logiciel libre et open source](https://www.developpez.com/actu/87401/Logiciel-libre-et-open-source-les-deux-concepts-sont-parfois-utilises-de-maniere-interchangeable-mais-quelle-est-la-difference/)
  - [Pourquoi l'expression « logiciel libre » est meilleure qu'« open source »](https://www.gnu.org/philosophy/free-software-for-freedom.fr.html)
 
**Linus Torvald**
  - [Wikipedia - Linus Torvalds](https://fr.wikipedia.org/wiki/Linus_Torvalds)
  - [Les excuse de Lunis Torvalds](https://www.lemonde.fr/pixels/article/2018/09/22/les-excuses-de-linus-torvalds-l-emblematique-et-caracteriel-fondateur-de-linux_5358713_4408996.html)

**Shell vs Bash**
  - [Wikipedia - Bourne-Again_shell](https://fr.wikipedia.org/wiki/Bourne-Again_shell)
  - [Difference between sh and bash](https://www.geeksforgeeks.org/difference-between-sh-and-bash/)

**Hacker : pirate ou bienfaiteur ?**
  - [Hackers ?](https://internetetmoi.fr/blog/hackers/index.html)
  - [Hacker vs pirate](https://www.secu-ordi.com/hacker-pirate/)
  - [Une brève histoire des hackers](https://usbeketrica.com/article/une-breve-histoire-des-hackers)

**GNU - Unix - Linux : Quel rapport ?**
  - [Wikipedia - Linux](https://fr.wikipedia.org/wiki/Linux_ou_GNU/Linux)
  - [Ubuntu - Kernel](https://doc.ubuntu-fr.org/kernel)
  - [What is the difference between Unix, Linux, BSD and GNU?](https://unix.stackexchange.com/questions/104714/what-is-the-difference-between-unix-linux-bsd-and-gnu)

 ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------

 # Unix - Linux

## Théorie  
**Le cours OpenClassRoom ( Ce cours concerne la partie 2 et 5 )**      
Se créer un compte openClassRoom (obligatoire): [Reprenez le contrôle à l'aide de Linux ! - OpenClassrooms](https://openclassrooms.com/fr/courses/7170491-initiez-vous-a-linux?archived-source=43538)     


**Quelques notions théoriques que vous pouvez synthétiser et compléter à partir du cours OpenClassRoom :**  
- Distributions Linux  
Quelle est la différence entre Unix, Linux, et Ubuntu ?  
	* Unix est le "coeur" commun à toutes les distributions.  
	* Une distribution, comme par exemple “Linux” et "Ubuntu", est une sorte d'extension d'Unix.


- Système de fichiers  
Dossier courant : Current Working Directory  
		C'est le dossier dans lequel vous êtes actuellement situé.  


- Dossier racine /  
Chemin absolu vs Chemin relatif  
	* Chemin absolu : commence toujours par ``` / ```. Un chemin absolu commence depuis la racine du disque dur.  
	* Chemin relatif : commence à partir de votre dossier courant  


- Votre dossier home  
	* C'est le dossier dans lequel vous êtes situé quand vous ouvrez un terminal  
	* C'est le seul dossier qui a un alias spécial ``` ~ ```    

 
- Permissions de fichiers  
Propriété de fichiers  
	* Les fichiers et les dossiers appartiennent tous à des utilisateurs et des groupes.
	* Lorsque vous créez un fichier, il vous appartient et vous avez tous les droits dessus. Ce n'est pas toujours le cas des autres fichiers.  
	* La préfixe de commande sudo permet souvent d'outrepasser les limites de permissions  

- Utilisateurs
	* Root  
	* Votre compte Utilisateur
	* Autres Utilisateur  

- Terminal et langage Bash  
	* Commandes bash  
		* Comment fonctionne une commande ?  
	* Langage bash  
		* Existe-t-il d'autres langages comme bash ?  
 
## Cheatsheet [à remplir]
### Fichiers
* Pour créer un répertoire et son répertoire parent
* Créer un répertoire
* Créer un répertoire dans un répertoire
* Renommer un fichier
* Changer le propriétaire d'un fichier
* Changer le groupe d'un fichier
* Changer le propriétaire et le groupe en même temps
* Changer les permissions d'un fichier
* Pour ouvrir un programme nano
* créer un fichier
* Créer un liens symbolique
### Dossiers
* Supprimer un répertoire
* Copier un dossier
* Liste tous les fichiers situés dans le dossiers
* Revenir au fichier/dossier précédent
* Suppression de répertoire
--------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Exercice pratique Linux

## Résumé  
Vous aurez besoin de précéder votre commande d'un “sudo” uniquement lorsque ce sera signalé dans une étape spécifique. 
Si vous devez l'utiliser ailleurs c'est probablement que c'est incorrect !  


**👉Ouvrez un terminal**
Vous êtes dans votre dossier home personnel.  
Créer un répertoire "exo" dans lequel vous allez ensuite créer un sous-répertoire "exo2".  
  - *🔎"how to make a directory in ubuntu"*
  - 🔥 {Achievement} Faites le d'une seule commande !  

**👉Créer un nouvel utilisateur "exo2user".** 
Vous n'avez pas besoin de créer le groupe, c'est fait automatiquement avec le user ( en syntaxe unix ca donne exo2user : exo2user )  
  - ❗❗ Vous devrez utiliser le préfixe sudo  
  - *🔎 "ubuntu create user with group"*
  - 🔥 {Achievement} Réussir d'une seule commande !  

**👉Ajoutez votre utilisateur courant au groupe "exo2user"**
  - ❗❗ Vous devrez utiliser le préfixe “sudo”  
  - Vous devrez redémarrer après avoir réussi la commande, pour que votre nouveau groupe soit pris en compte  
  - *🔎 "ubuntu add existing user to group"*

**👉Rouvrez un terminal après avoir redémarré.**
Avant d'aller plus loin, vérifiez que vous appartenez au groupe "exo2user" avec la commande `groups`  

**👉Aller dans votre répertoire "exo2", toujours avec le terminal en utilisant la commande `cd`
  - *🔎"ubuntu change directory"*
  - Une fois dans le dossier utilisez la commande `ls -al`  

**👉Changez les droits de votre répertoire courant "exo2" de façon à ce qu'il appartienne à l'utilisateur "exo2user" et au groupe "exo2user"**
  - ❗❗ Attention : vous allez exécuter la commande la plus sensible de tout l'exercice. 
  - Il ne faut surtout pas que votre commande chmod soit suivie d'un slash / ( chemin absolu ).  
  - *🔎"ubuntu change directory owner"*  

**👉Ajoutez les permissions d'écriture permettant au groupe "exo2user" de modifier le dossier courant.**
  - *🔎"ubuntu chmod tutorial"*

**👉Remonter d'un niveau avec la commande cd .. de façon à vous retrouver dans le dossier "exo".**
  - Vérifiez votre dossier courant avec la commande pwd.
  - Vous devriez être dans le dossier suivant : /home/<votre-user>/exo
  - 🔥 {Achievement} J'ai compris le lien entre la commande cd, pwd, et le dossier courant  

**👉Créer un lien symbolique depuis "exo2" vers "exo2-symbolique"** 
  - ❗❗ Vous devrez utiliser le préfixe sudo  
  - Votre commande ne doit contenir aucun slash /  
  - *🔎 "ubuntu create symbolic link"*
  - 🔥 {Achievement} J'ai compris la différence entre lien symbolique et fichier  

**👉Aller dans votre répertoire "exo2-symbolique"**

**👉Dans ce dossier, créer un fichier "prog.sh" en mode édition. avec le programme `nano`.**
  - Une fois dans l'éditeur nano , vous pouvez déclencher les raccourcis en bas de l'écran avec la touche CTRL  
  - Vous allez créer votre premier programme Bash !
  - Cherchez un exemple de programme Bash "hello world" sur google puis copiez ce programme
  - Utilisez la commande chmod +x prog.sh pour rendre votre programme executable
  - Exécutez votre programme avec la commande ./prog.sh
  - Votre programme devrait afficher "Hello, World"
    
**👉Retournez à la racine de votre dossier "exo". Listez le contenu avec `ls -alR`, puis faites une capture d'écran de votre terminal et envoyez-la au formateur**
  - 🔥 {Achievement} Aider au moins 2 collègues à remplir un {Achievement}  
