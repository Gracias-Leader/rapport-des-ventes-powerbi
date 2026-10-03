# 📊 Synthèse des ventes — Rapport Power BI

Rapport Power BI de suivi des ventes, des revenus et de la marge bénéficiaire, publié dans le **service Power BI**, diffusé via un **tableau de bord épinglé**, **alertes** et **abonnements par e-mail**, et consultable sur **Power BI Mobile**.

> Projet réalisé avec Power BI Desktop et Power BI Service.

---

## 🎯 Objectif

Donner une vue claire et à jour de la performance commerciale :

- Quelles quantités sont vendues, et pour quels produits ?
- Quels pays pèsent le plus dans les ventes et la marge ?
- Comment évoluent les ventes médianes et la marge dans le temps ?
- Où en est le bénéfice cumulé de l'année (YTD) ?

---

## 🗂️ Contenu du rapport

Le fichier `Synthèse_des_ventes.pbix` contient **2 pages** :

### Page 1 — Vue du rapport

| Visuel | Rôle |
|---|---|
| Cartes (KPI) | Stock, quantités achetées, bénéfice trimestriel, bénéfice cumulé YTD, marge bénéficiaire annuelle, ventes médianes |
| Histogramme groupé | Quantité vendue par produit |
| Barres groupées | Points de fidélité par pays |
| Graphique en secteurs | Répartition médiane des ventes par pays |
| Courbe | Ventes médianes au fil du temps (axe calendrier) |
| Segment (slicer) | Filtre par pays |

### Page 2 — Synthèse des bénéfices

| Visuel | Rôle |
|---|---|
| Cartes / KPI | Bénéfice annuel, revenu net USD, revenu brut USD (avec tendance mensuelle) |
| Barres groupées | Revenu net par produit |
| Graphique en aires | Marge bénéficiaire annuelle au fil du temps (par mois) |
| Anneau | Marge bénéficiaire annuelle par pays |
| Tableau | Détail : produit, catégorie, pays, quantité, stock, prix brut, revenu brut, revenu net |
| Segment (slicer) | Filtre par date |

---

## 🧱 Modèle de données

- **`Sales in USD`** — table de faits (produits, catégories, pays, quantités, stock, prix, revenus brut/net, points de fidélité)
- **`CalendarTable`** — table calendrier pour l'analyse temporelle (date, mois)

**Mesures DAX utilisées :**

- `Ventes médianes`
- `Bénéfice trimestriel`
- `Bénéfice cumulé YTD`
- `Marge Bénéficiaire annuelle`

---

## ☁️ Déploiement dans Power BI Service

### 1. Publication
Le rapport a été publié depuis Power BI Desktop vers un espace de travail du service Power BI (*Accueil → Publier*).

### 2. Épinglage au tableau de bord
Les visuels clés (cartes KPI, graphiques principaux) ont été **épinglés** sur un tableau de bord afin de regrouper les indicateurs essentiels sur une seule page, actualisée automatiquement avec les données du rapport.

### 3. Alertes de données
Des **alertes** ont été créées sur les tuiles du tableau de bord (cartes/KPI). Elles envoient une notification lorsqu'une valeur franchit un seuil défini.

- Indicateurs surveillés : bénéfice cumulé YTD, ventes médianes]
- Seuils : 400
- Fréquence de notification : `[à compléter]`

> ℹ️ Les alertes ne fonctionnent que sur les tuiles d'un **tableau de bord** de type carte, jauge ou KPI. C'est la raison de l'étape d'épinglage.

### 4. Abonnements
Des **abonnements** ont été définis pour recevoir automatiquement par e-mail un aperçu du rapport/tableau de bord.

- Fréquence : quotidien
- Destinataires : Adventure Works

### 5. Version mobile
Le rapport a été adapté à l'affichage **Power BI Mobile** (mise en page mobile : visuels réorganisés en colonne pour l'écran du téléphone), ce qui permet de consulter les indicateurs et de recevoir les alertes en déplacement.

---

## 🛠️ Technologies

- Power BI Desktop
- Power BI Service (publication, tableau de bord, alertes, abonnements)
- Power BI Mobile
- DAX

---


## 👤 Auteur

**Bertin** — Data Analyst
GitHub : [Gracias-Leader](https://github.com/Gracias-Leader) · LinkedIn : Gracias-NDEMA
