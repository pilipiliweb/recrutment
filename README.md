# Tâches
- [ ] Initialisation d'un projet symfony

- [ ] Création d'un base de donnée

- [ ] Créer une entity product

- [ ] Créer une entity brand

- [ ] Créer une fixture pour ajouter 3/4 marques (Adidas, Nike, Puma, Carhartt)

- [ ] Mettre des messages flash lors de la validation d'une action formulaire

- [ ] Rendre traductible les messages flash

- [ ] Créer une page d'accueil affichant que les produits activés

- [ ] Créer une page avec la liste des produits actif ou non

- [ ] Intégrer un éditeur avancé dans le champ description (https://alex-d.github.io/Trumbowyg/documentation/#installation)

- [ ] Créér une page d'ajout et/ou d'édition avec un enregistrement dans les logs

- [ ] Créer une commande symfony de gérer l'activation des produits avec l'envoie d'un mail

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
| created_at  | datetime    | NO   |     | NULL    |                |
| updated_at  | datetime    | YES  |     | NULL    |                |

## Brand

| Field | Type        | Null | Key | Default | Extra          |
| ----- | ----------- | ---- | --- | ------- | -------------- |
| id    | int         | NO   | PRI | NULL    | auto_increment |
| name  | varchar(55) | NO   |     | NULL    |                |

# Bonus

- [ ] Indiquer la ligne de commande pour mettre en tâche cron la commande symfony

# Note

Il y a une incompatibilité avec les version Jquery bootstrap et l'éditeur Trumbowyg
