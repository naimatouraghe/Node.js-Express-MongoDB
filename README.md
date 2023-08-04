# Node.js-Express-MongoDB

Tp projet web full-stack

## Partie 1

- Node peut être installé à partir de NodeJS.org.

-L'application front-end pour ce cours peut être clonée avec git clone , installée avec npm install , et lancée avec npm run start

## Partie 2

- Les projets Node sont initialisés avec la commande npm init .

- Un serveur Node basique est démarré avec la méthode createServer du package http .

- Nodemon est un package qui mettra à jour votre serveur démarré à chaque changement de fichier, vous facilitant le développement Node.

## Partie 3

- Le framework Express est installé et enregistré dans le package.json avec npm install express .

- Pour créer une application Express, appelez simplement la méthode express() .

- Un middleware est un bloc de code qui traite les requêtes et réponses de votre application.

- Ajouter la normalisation de port, la gestion d'erreur et du logging basique à votre serveur Node le rend plus constant et plus facile à déboguer.

## Partie 4

- La méthode app.use() vous permet d'attribuer un middleware à une route spécifique de votre application.

**Focus CORS**

- Le CORS définit comment les serveurs et les navigateurs interagissent, en spécifiant quelles ressources peuvent être demandées de manière légitime – par défaut, les requêtes AJAX sont interdites.

Il s'agit d'un système de sécurité qui, par défaut, bloque les appels HTTP entre des serveurs différents, ce qui empêche donc les requêtes malveillantes d'accéder à des ressources sensibles.

Dans notre cas, nous avons deux origines : localhost:3000 et localhost:4200, et nous souhaiterions qu'elles puissent communiquer entre elles. Pour cela, nous devons ajouter des headers à notre objet response.

- Pour permettre des requêtes cross-origin (et empêcher des erreurs CORS), des headers spécifiques de contrôle d'accès doivent être précisés pour tous vos objets de réponse.
