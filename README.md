####################################
N'OUVREZ QUE git-bash.exe !!!!!!!!!!
####################################

______________________________________________________________________
Toute la conf et le code se trouvent dans le fichier ./etc/bash.bashrc
----------------------------------------------------------------------

Dans le cas d'une installation de zéro, si vous en avez le rôle :
1. Faire une copie du fichier des expressions en le renommant, même à la racine ou dans un sous-répertoire : le .gitignore ne le prendra pas en charge.
2. Récupérer la dernière version du fichier des expressions et la mettre à la racine du dossier principal (\\pprod-pfm-qlik-file\EMAT-BGPS_TdB-CEMAT\1_DASHBOARD\00_DASHBOARD_INCLUDE par défaut)
3. Modifiez la configuration du script
4. Lancez git-bash.exe, il risque d'y avoir des erreurs. Si toutes celles concernant la conf sont corrigées, il restera l'initialisation de la forge et du dossier
5. Lancez clessh pour avoir votre clessh
5. bis. Si clessh ne remonte rien, lancez initssh
6. Ajoutez votre clé ssh à votre profil forge
6. Lancez initdossieremat, ça initialise tout, y compris le local.

Dans le cas d'une utilisation classique avec tout configuré par celui en ayant le rôle :
1. Laissez-vous guider sur la conf initiale, il y a peu à faire mais tout doit être bien fait.
Si le script tourne en boucle sur la conf c'est qu'elle n'est pas bonne. Il y a un minimum de tests faits dessus au démarrage.
2. Si la conf est bonne le script se charge de tout initialiser, vous perdrez toute modification préalable au lancement. Faites des save !


Utilisation au quotidien :
1. Lancez git-bash.exe
2. Il lance tout seul le fichier excel.
3. Dès que vous en avez le temps et l'envie, faites un save. Basez-vous sur l'interface du notepad pour rédiger vos modifs. PAS DE SAUTS DE LIGNE
4. N'oubliez pas de pousser à distance avec partage. 
5. A chaque démarrage du script, tout est réinitialisé pour limiter le risque de conflits. Si vous voulez garder des modifs, au démarrage du script vos dernières modifs sont placées dans le fichier Version_précédente_$nomfichier. Ce fichier ne sera jamais poussé en-dehors de votre répertoire local
