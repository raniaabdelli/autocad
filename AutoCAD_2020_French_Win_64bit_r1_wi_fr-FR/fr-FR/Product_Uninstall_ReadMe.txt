-----------------------------
Fichier Readme de la désinstallation de produits
-----------------------------

Les instructions qui suivent expliquent comment désinstaller des produits à partir d'une répartition. Pour résumer la procédure, vous devez d'abord convertir le fichier <nom répartition>_Uninstall.txt en un fichier de traitement par lors au format ANSI. Ouvrez ensuite ce fichier et sélectionnez les produits à désinstaller en supprimant les marques de commentaires situées sur les lignes de commande applicables. Enfin, exécutez le fichier de traitement par lots pour désinstaller les produits.
 
La procédure détaillée est la suivante :

1. Dans le dossier de répartition, ouvrez le fichier<nom répartition>_Uninstall.txt dans le Bloc-notes ou dans un éditeur de texte similaire. 

2. Cliquez sur Enregistrer sous. Dans la liste Codage, sélectionnez ANSI, puis modifiez l'extension de fichier en .bat. Le nom de fichier recommandé est <nom répartition>_Uninstall.bat. Notez que le codage ANSI est requis pour créer un fichier de traitement par lots exécutable.

3. Ouvrez le fichier de traitement par lots et activez les commandes de désinstallation en supprimant les caractères "::" au début de la ligne de commande "::call :funcUninstall" correspondant à chaque produit que vous souhaitez désinstaller.

4. Exécutez le fichier de traitement par lots avec des droits d'administrateur.