# PySpark OpenFoodFacts ETL

Ce projet vise à créer une solution ETL en utilisant Apache Spark (PySpark) pour extraire, transformer et charger des données à partir d'OpenFoodFacts. L'objectif principal est de générer des menus hebdomadaires en utilisant les produits disponibles dans la base de données OpenFoodFacts, puis d'importer ces menus dans une base de données SQLite3.

## Objectifs du Projet

1. **Collecte de Données :** Extraire des données d'OpenFoodFacts ainsi que d'autres sources liées aux programmes alimentaires et aux informations sur les utilisateurs.

2. **Génération de Menus :** Utiliser les données collectées pour générer des menus hebdomadaires de manière aléatoire. Les menus doivent refléter la diversité des produits disponibles dans la base de données OpenFoodFacts.

3. **Équilibre Nutritionnel :** Assurer que les menus générés respectent l'équilibre nutritionnel en fonction des informations spécifiées dans le programme alimentaire de l'utilisateur.

4. **Importation dans SQLite3 :** Charger les menus générés dans une base de données SQLite3 pour permettre une intégration aisée avec d'autres applications.

## Configuration du Projet

1. **Environnement Virtuel :** Créez un environnement virtuel pour isoler les dépendances du projet.

    ```bash
    python3 -m venv venv
    source venv/bin/activate  # Pour Linux/Mac
    # ou
    .\venv\Scripts\activate   # Pour Windows
    ```

2. **Installation des Dépendances :** Installez les dépendances requises en utilisant le fichier `requirements.txt`.

    ```bash
    pip install -r requirements.txt
    ```

3. **Configuration Spark :** Assurez-vous d'avoir une installation de Spark fonctionnelle. La configuration peut varier en fonction de votre environnement.

4. **Base de Données SQLite3 :** Créez une base de données SQLite3 pour stocker les menus générés.

    ```bash
    sqlite3 openfoodfacts_menus.db < schema.sql
    ```

## Utilisation

1. **Notebook ETL :** Utilisez le notebook `files/etl_process.ipynb` pour exécuter l'extraction, la transformation et le chargement des données en une seule séquence.

## Contributions et Licence

Les contributions sont les bienvenues. N'hésitez pas à ouvrir une issue ou une pull request. Ce projet est sous licence [MIT](LICENSE).
