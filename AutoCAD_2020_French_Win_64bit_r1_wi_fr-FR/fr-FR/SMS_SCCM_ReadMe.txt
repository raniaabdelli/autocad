Fichier Readme relatif à l'intégration de SMS et SCCM
Les améliorations apportées à la technologie de répartition d'Autodesk® permettent à bon nombre d'administrateurs de rationaliser leurs processus d'intégration des répartitions Autodesk sous Microsoft® Systems Management Server (SMS) et System Center Configuration Manager (SCCM). Dans la plupart des cas, les répartitions Autodesk peuvent désormais être annoncées à l'aide d'une seule ligne de commande, au lieu de plusieurs lignes de commande pour chaque composant de la répartition. 
Pour annoncer une répartition avec une seule ligne de commande, utilisez la syntaxe suivante :
.\Img\Setup.exe /W /Q /I.\Img\<nom de la répartition>.ini /language fr-fr
Cet exemple de ligne de commande suppose que le contenu du package est défini au niveau du dossier racine du dossier de répartition du produit Autodesk et que la langue du produit est le français (fr-fr).

Si vous avez créé une répartition combinée et souhaitez la publier, utilisez la syntaxe suivante:
.\img\Setup.exe /w /x86 <adminImage's name> /x64 <adminImage's name>

Configuration logicielle requise
Avant de créer une annonce SCCM, assurez-vous que Microsoft .NET Framework 4.0 est installé sur tous les ordinateurs cibles. Direct X doit être installé sur les ordinateurs Windows XP avant que ceux-ci ne reçoivent une annonce relative à un produit Autodesk 2011 ou ultérieur.

Annonce au niveau du composant
Dans certains cas spécifiques, tels que des limites de délai d'exécution, il se peut que vous deviez annoncer une répartition Autodesk au niveau du composant. Reportez-vous à <nom de la répartition>_SCCM.txt pour obtenir la liste des lignes de commande requises dans l'ordre dans lequel elles doivent être exécutées sur les ordinateurs cibles. Ces commandes varient en fonction de la répartition. Pour les longues lignes de commande, utilisez un fichier de commandes.
Pour plus d'informations sur la technologie de répartition d'Autodesk et son intégration à SMS et SCCM, reportez-vous au Guide de l'administrateur réseau fourni avec votre produit Autodesk.
