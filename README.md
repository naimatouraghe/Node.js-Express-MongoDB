# Node.js-Express-MongoDB

Tp projet web full-stack

front-end: npm run start
back-end : nodemon start

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

Dans notre cas, nous avons deux origines : localhost:3000 et localhost:4200, et nous souhaiterions qu'elles puissent communiquer entre elles. Pour cela, nous devons ajouter des headers spécifiques de contrôle d'accès doivent être précisés pour tous vos objets de réponse.

## Partie 5

En passant votre middleware à app.post() au lieu de app.use() , il répondra uniquement aux requêtes de type POST.

**Veillez à :**

- soit modifier la méthode use en get pour le middleware des requêtes GET ;

- soit placer la route POST au-dessus du middleware pour les requêtes GET, car la logique GET interceptera actuellement toutes les requêtes envoyées à votre endpoint /api/stuff , étant donné qu'on ne lui a pas indiqué de verbe spécifique. Placer la route POST au-dessus interceptera les requêtes POST, en les empêchant d'atteindre le middleware GET.

## Partie 6 - QCM

1. En créant un serveur HTTP avec Node, on utilise la fonction createServer() . On peut passer une fonction à createServer() qui réagira aux requêtes entrantes. Quels arguments reçoit cette fonction passée ?

2. Dans une application Express, que doit faire le dernier middleware pour une route donnée pour empêcher les requêtes d'expirer ?

3. À quoi sert la fonction next() ?

4. Un code HTTP de 200 représente généralement :

5. Un code HTTP de 201 représente généralement :

6. Une erreur CORS peut survenir quand :

7. Quelle méthode permet d'empêcher des erreurs CORS ?

8. Le package body-parser :
