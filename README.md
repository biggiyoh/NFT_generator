faire un clone dans le dossier que vous voulez
dans ce dossier vous aurez un dossier layers, dans celui ci mettez vos layers et renomez chaque dossier de layer comme vous le voulez,
par exemple helices pour le dossier ou vous allez mettre les layers d'helices, background pour les backgrounds etc....
pour chaque layers renommez (ex : Shuriken blades pour les ventilo shuriken etc....) et a la fin ajouter # + un chiffre
qui correspondra au pourcentage de chance aue ce layer as de chance de tomber. 
Exemple : le layer nommé Shuriken Blades#10  aura 10% de chances de tomber !

Ensuite ouvrez le dossier complet avec Visual studio code
ouvrez le fichier config.js qui se trouve dans ./src

En dessous j'explique un peu en details les lignes qu'on utilisera, mais pour les tests elles sont pas toutes utiles. Vous pouvez les lire pour comprendre pour la suite si vous voulez ;)
Les lignes qui vous seront utiles pour les tests sont les Lignes : 27, 29, 45 a 47 

Ligne 8 : Nom du NFT qui sera suivit de son numero lors de la generation (pas utile pour les tests)
Ligne 9 : une description qui apparaitra dans la description du NFT (et dans les metadonnées) (pas utile pour les tests)
Ligne 13 : le symbol de la collection (pas utile pour les tests)
Ligne 14 : Définir les Royalties, 1000=10% (pas utile pour les tests)
Ligne 15 : Un lien qui apparaitra dans la description du NFT (pas utile pour les tests)
Ligne 18 : Adresse wallet qui recoit les crypto quand quelqu'un achete un nft (pas utile pour les tests)
Ligne 19 : le pourcentage que l'adresse au dessus recoit (on peut mettre plusieurs adresses si on veut split les revenus des vente de NFT direcement au lieu de le faire nous apres) (pas utile pour les tests)
Ligne 27 : Nombre de NFT a généré (celle la elle est pour toi nicooowww)
Ligne 29 : Liste des catégories de layers DANS l'ordre. Si vous en avez plus rajoutez des ligne etc .... Les noms doivent correspondre au nom du dossier dans le quel se trouve les layers (par exemple nous on aura un dossier Hélices), et tres important l'ordre car c'est l'ordre de superposition des layers de haut en bas de la liste !
Lignes 45 a 47 : Taille et effet des NFT générés 
Lignes 50 a 54 : Si on veut faire des Gif, mettre export: true et remplir les caracteristique en dessous (pas utile pour les tests)
Lignes 70/71 : Si on veut que nos NFT sortent en pixel ratio = le ratio de pixel qu'on veut (pas utile pour les tests)
Lignes 74 a 78 : On peut modifier les caracteristiques basique du background (pas utile pour les tests)
Ligne 81 : Si on veut rajouter des metadata externes a celles propres aux layers (pas utile pour les tests)
Ligne 83 : Limiter une rareté (pas utile pour les tests)

une fois vos configurations faites, ouvrez un terminal
installez Node.js 
installer yarn (normalement deja compris dans la derniere version stable de Node.js)
j'ai eu des soucis de permissions avefc yarn donc soyez sur d'etre sur un compte admin et d'ouvrir VS code en tant qu'admin, si ca s'installe toujours pas tapez corepack enable pour activer la totalité des fonctions de yarn et ensuite refaites yarn install

rendez-vous dans le dossier de generation : cd ./NFT_generator
executez la commande yarn install
puis npm install pour etre sur que tout est bien installé

ensuite vous avez juste a executer la commande node index.js pour lancer la génération
une fois la génération terminée vous retrouver une fichier build qui s'est crée et qui contient un dossier image (les NFT générés et un dossier json qui contient les metadata attachées aux images)

Enjoy les coupaings !
