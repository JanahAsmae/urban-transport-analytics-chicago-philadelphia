# 🚇 Urban Transport Analytics — Chicago & Philadelphia

## 📌 Contexte du projet

Ce projet s’inscrit dans une démarche d’**analyse décisionnelle (Business Intelligence)** appliquée aux **transports urbains** des villes de **Chicago** et **Philadelphia**.

L’objectif principal est d’analyser les **tendances du ridership (fréquentation)** selon :

- le **mode de transport** (Bus, Rail, etc.)
- les **routes**
- la **dimension temporelle** (mensuelle, annuelle)
- la **comparaison inter-villes**

Le projet couvre l’ensemble du **cycle BI** :

- planification et suivi (**Jira**)
- préparation et structuration des données  
- modélisation en étoile  
- création de mesures DAX  
- conception de dashboards analytiques dans **Power BI**  
- documentation du projet (**Confluence**, **GitHub**)

---

## 🎯 Objectifs analytiques

- Comparer l’évolution du ridership entre **Chicago** et **Philadelphia**
- Identifier les **modes de transport dominants**
- Analyser les **routes les plus fréquentées**
- Mesurer la **croissance mensuelle (MoM)** et **annuelle (YoY)**
- Évaluer la **volatilité du ridership par route**
- Fournir des **indicateurs clairs** pour l’aide à la décision

---

## 🧱 Modélisation des données

Le projet repose sur un **modèle en étoile (Star Schema)** composé de :

### Tables de faits
- **Fact_Ridership_Mode** : analyse du ridership par **mode**
- **Fact_Ridership_Route** : analyse du ridership par **route**

### Tables de dimensions
- **Dim_Date** : temps (année, mois)
- **Dim_City** : ville (Chicago, Philadelphia)
- **Dim_Mode** : mode de transport
- **Dim_Route** : routes

👉 Cette séparation garantit :

- des **mesures DAX cohérentes**
- une **bonne performance**
- une **lecture claire** pour les dashboards

---

## 📊 Dashboards réalisés

### 1️⃣ Dashboard — Analyse par Mode
- Ridership total par mode  
- Comparaison **Chicago vs Philadelphia**  
- Croissance **MoM & YoY**  
- Contribution de chaque mode  
- Évolution temporelle  

### 2️⃣ Dashboard — Analyse par Route
- Top routes par fréquentation  
- Volatilité du ridership  
- Évolution temporelle par route  
- Comparaison inter-villes  
- Classement des routes  

---

## 📁 Structure du projet

```bash
.
├── data
│   ├── raw
│   │   ├── Avg_By_Mode_Chicago.xlsx
│   │   ├── Avg_By_Mode_Philadelphia.xlsx
│   │   ├── Avg_By_Route_Chicago.xlsx
│   │   ├── Avg_By_Route_Philadelphia.xlsx
│   │   └── ...
│   └── processed
│       ├── rdf_CTA_Ridership_Daily_*.csv
│       └── ...
│
├── notebooks
│   └── data.ipynb
│
├── scripts
│   └── (scripts pour convertir les fichiers rdf en csv)
│
├── documentation
│   ├── Plan_projet_confluence.png
│   ├── Planification_jira.png
│   └── documentation_espace_confluence.png
│
├── powerbi
│   └── Chicago_Philadelphia_transport_analytics.pbix
│
└── README.md
```
## 🧪 Données

Les données utilisées sont issues de fichiers **CSV / Excel** représentant :

- le **ridership journalier moyen**
- agrégé par **mode**, **route**, **ville** et **temps**

Les données sont **nettoyées et structurées** avant leur intégration dans **Power BI**.

---

## 🧠 Mesures DAX clés

- Ridership total (**Mode / Route**)
- Croissance **MoM (%)**
- Croissance **YoY (%)**
- Contribution par mode (**%**)
- Part de chaque ville
- Classement des routes
- Volatilité du ridership

👉 Toutes les mesures respectent le **grain de chaque table de faits**.

---

## 🛠️ Outils & Technologies

- **Power BI** — Visualisation & DAX  
- **Excel / CSV** — Sources de données  
- **Python (Jupyter Notebook)** — Préparation et exploration  
- **GitHub** — Versioning et collaboration  
- **Confluence** — Documentation projet  
- **Jira** — Planification et suivi  

---

## 📄 Documentation

- Documentation du **modèle de données**
- Explication des **mesures DAX**
- Planification du projet (**Jira**)
- Présentation des dashboards (**Confluence**)

---

## 👩‍💻 Auteur

**Janah Asmae**  
🎓 Licence Informatique, Réseaux & Multimédia  
📊 Data Analytics  
🌍 Casablanca, Maroc  

---

## ✅ Statut du projet

- ✔ Modélisation terminée  
- ✔ Mesures DAX validées  
- ✔ Dashboards finalisés  
- ✔ Documentation complétée  

