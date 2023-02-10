# 🚀 Workshop: Construisez une webapp avec l'API IPFS et une API reposant sur IPFS

Bienvenue à ce workshop, où nous allons vous montrer comment construire une webapp en utilisant l'API IPFS et construire une API reposant sur IPFS.
Ce workshop est découpé en 6 étapes faciles à suivre. Nous sommes convaincus que, à la fin de ce workshop, vous serez en mesure de construire votre propre webapp en utilisant IPFS.

## Pré-requis 
- Connaissances de base en développement web (HTML, CSS, JavaScript)
- Connaissances en utilisation de l'API REST
- Connaissance de l'IPFS et de son fonctionnement

## Étape 1: Configurer votre environnement de développement
1. Installez Node.js sur votre ordinateur
2. Installez les dépendances IPFS en utilisant la commande `npm install ipfs`
3. Avoir un noeud IPFS Kubo sur sa machine
4. Installer le framework front de votre choix

## Étape 2: Créer un projet front de votre choix et soyez créatif sur la partie front (on ne s'attarde pas dessus, c'est pas important)
1. En autonomie, prendre 15-25min à choisir quelle type de donnée voulez vous que votre site délivre. (ex: photo, text etc..)

## Étape 3: Créer votre API
1. Créer un dossier `backend` dans lequel vous ferez votre API pour intéragir avec votre noeud IPFS.
2. Connectez votre webapp à l'API IPFS en utilisant la méthode `ipfs.init()`
3. Vérifiez que la connexion à l'API IPFS est établie en utilisant la méthode `ipfs.version()`
4. Lisez attentivement la documentation et séléctionner les méthodes dont vous aurez besoins pour votre web-app

## Étape 4: Ajouter des fichiers à IPFS
1. Créez un fichier example.txt dans votre dossier de projet
2. Ajoutez ce fichier à IPFS. (vous pouvez completement stocker le CID de votre fichier sur une databse like postgresql pour avoir toujours vos contenus de disponible
3. Récupérez l'adresse IPFS de ce fichier en utilisant la méthode `ipfs.files.cat()`

## Étape 5: Utiliser express pour créer un server avec lequel votre front pourra communiquer
1. Créez un fichier api.js pour votre code d'API
2. Créez une nouvelle instance IPFS dans votre fichier api.js
3. Écrivez une méthode pour ajouter des données à IPFS en utilisant la méthode `ipfs.files.add()
