# Tâches
- [ ] Initialisation d'un projet symfony

- [ ] Création d'une base de donnée

- [ ] Créer une entity product

- [ ] Créer une entity brand

- [ ] Créer une fixture pour ajouter 3/4 marques (Adidas, Nike, Puma, Carhartt)

- [ ] Mettre des messages flash lors de la validation d'une action formulaire

- [ ] Rendre traductible les messages flash

- [ ] Créer une page d'accueil affichant que les produits activés

- [ ] Créer une page avec la liste des produits actif ou non

- [ ] Intégrer un éditeur avancé dans le champ description (https://alex-d.github.io/Trumbowyg/documentation/#installation)

- [ ] Créér une page d'ajout et/ou d'édition avec un enregistrement dans les logs

- [ ] Créer une commande symfony pour gérer l'activation des produits avec l'envoie d'un mail et le lien sur la page listing produit

# Entités

- Générer un slug unique pour le produit en automatique

## Product

| Field       | Type        | Null | Key | Default | Extra          |
| ----------- | ----------- | ---- | --- | ------- | -------------- |
| id          | int         | NO   | PRI | NULL    | auto_increment |
| brand_id    | int         | NO   | MUL | NULL    |                |
| name        | varchar(55) | NO   |     | NULL    |                |
| description | longtext    | YES  |     | NULL    |                |
| price       | double      | NO   |     | NULL    |                |
| enabled     | tinyint(1)  | NO   |     | NULL    |                |
| slug        | varchar(70) | NO   | UNI | NULL    |                |
| created_at  | datetime    | NO   |     | NULL    |                |
| updated_at  | datetime    | YES  |     | NULL    |                |

## Brand

| Field | Type        | Null | Key | Default | Extra          |
| ----- | ----------- | ---- | --- | ------- | -------------- |
| id    | int         | NO   | PRI | NULL    | auto_increment |
| name  | varchar(55) | NO   |     | NULL    |                |

# Bonus

- [ ] Intégrer le package de cookie et changer le style du bouton en vert et rendre traductible les champs

- [ ] Créer une page cookie avec un contenu et modifier le template pour que le lien en savoir plus redirige vers la page de politique cookie

- [ ] Indiquer la ligne de commande pour mettre en tâche cron la commande symfony

# Note

Il y a une incompatibilité avec les version Jquery bootstrap et l'éditeur Trumbowyg

# Librairie

Bootstrap

https://getbootstrap.com/docs/4.5/getting-started/introduction/

Pour générer un slug

https://github.com/cocur/slugify

Pour les cookies

https://github.com/ConnectHolland/cookie-consent-bundle
