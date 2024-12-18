**Cahier des Charges pour une Application Java et Angular : Consultation des Données Boursières**

---

## 1. Contexte et Objectifs
L'objectif de ce projet est de développer une application web permettant de consulter et d'analyser les données boursières en temps réel. L'application utilisera une architecture backend en Java (Spring Boot) et un frontend en Angular. Les données seront récupérées à partir d'une API boursière publique, comme Alpha Vantage ou Yahoo Finance.

---

## 2. Spécifications Fonctionnelles

### 2.1 Fonctionnalités Principales
- **Consultation des Marchés Boursiers** :
  - Affichage des indices boursiers principaux (CAC40, NASDAQ, etc.).
  - Affichage des actions les plus performantes et celles en baisse.

- **Recherche et Filtrage** :
  - Recherche par symbole d'action ou nom d'entreprise.
  - Filtrage par secteur ou performance.

- **Détails d’une Action** :
  - Affichage du cours actuel, de la variation, et des volumes.
  - Historique des cours sur une période donnée (7 jours, 1 mois, 1 an).

- **Graphiques** :
  - Visualisation des données historiques sous forme de graphiques interactifs.

### 2.2 Fonctionnalités Complémentaires
- **Watchlist** :
  - Permettre à l'utilisateur de sélectionner et suivre des actions spécifiques.

- **Notifications** :
  - Alerte sur les variations importantes (>5%) des actions de la Watchlist.

---

## 3. Spécifications Techniques

### 3.1 Frontend
- **Technologie** : Angular.
- **Langage** : TypeScript, HTML, SCSS.
- **Bibliothèques** :
  - Angular Material pour le design.
  - Chart.js ou Highcharts pour les graphiques interactifs.
  - RxJS pour la gestion des flux de données.

### 3.2 Backend
- **Technologie** : Java avec Spring Boot.
- **Base de Données** : PostgreSQL pour stocker les watchlists et les données persistantes.
- **API externe** :
  - Intégration avec Alpha Vantage ou Yahoo Finance pour récupérer les données boursières en temps réel.

### 3.3 Infrastructure
- **Hébergement** :
  - En local pour le développement et les tests.

---

## 4. User Stories

### Utilisateur : Anonyme
1. **En tant qu'utilisateur, je veux voir une liste des indices boursiers principaux**
   - Critères d'acceptation :
     - Les indices (nom, valeur, variation) sont affichés dans une liste dynamique.

2. **En tant qu'utilisateur, je veux rechercher une action par nom ou symbole**
   - Critères d'acceptation :
     - Les résultats s'affichent dynamiquement en fonction de la saisie.

3. **En tant qu'utilisateur, je veux consulter les détails d'une action**
   - Critères d'acceptation :
     - Les détails incluent le cours actuel, la variation, et un graphique historique.

4. **En tant qu'utilisateur, je veux suivre certaines actions**
   - Critères d'acceptation :
     - Les actions suivies apparaissent dans une section "Watchlist".

5. **En tant qu'utilisateur, je veux voir les performances des actions sous forme de graphique**
   - Critères d'acceptation :
     - Les graphiques sont interactifs et affichent les données correctement.
