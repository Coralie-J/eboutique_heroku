# eboutique_symfony

## Structure de l'application

L'application utilise le framework Symfony et son système de rôles. Elle est utilise 2 rôles : celui du nom de
"ROLE_USER" qui est le rôle par défaut de tous les utilisateurs connectés, en plus il y a le rôle nommé "ROLE_ADMIN"
qui offre un accès administrateur.

## Fonctionnalités de l'application web

En tant qu'utilisateur non-connecté, vous pourrez voir ajouter des produits dans votre panier, créer un compte
ou voir les description des différents produits. Vous pourrez également mettre à jour le nombre d'exemplaires pour chaque
produit que vous souhaitez dans votre panier. C'est seulement une fois connecté que vous pourrez effectuer vos commandes.


En tant qu'administrateur, en plus de toutes les fonctionnalités offertes en étant utilisateur vous aurez normalement à la connexion
2 items en plus dans le menu principal, pour gérer les catégories et les produits. Il vous sera possible de créer des catégories, des produits, de mettre leurs propriétés à jour.

## Bugs et erreurs

- Lorsqu'on se déconnecte après avoir ajouté des produits dans son panier, le panier se vide.
Ceci est dû au fait que quand on se déconnecte, Symfony supprime la session.

- Une autre chose, on ne peut pas changer de mot de passe.

## Routes

### - /home

C'est la route principale du projet. On y voit tous les produits disponibles.

### - /user/login

Route de connexion qui utilise l'authentification Symfony pour authentifier un utilisateur.

### - /panier/