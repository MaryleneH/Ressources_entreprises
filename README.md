# 📊 Formation aux Statistiques d'Entreprises

> Une formation complète, moderne et pédagogique aux statistiques officielles sur les entreprises — basée sur [Quarto](https://quarto.org), [l'INSEE](https://www.insee.fr), [Eurostat](https://ec.europa.eu/eurostat) et [data.gouv.fr](https://www.data.gouv.fr).

[![Deploy to GitHub Pages](https://github.com/MaryleneH/Ressources_entreprises/actions/workflows/publish.yml/badge.svg)](https://github.com/MaryleneH/Ressources_entreprises/actions/workflows/publish.yml)
[![Quarto](https://img.shields.io/badge/Quarto-1.5+-blue?logo=quarto)](https://quarto.org)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

---

## 🌐 Site web

Le site est disponible à l'adresse :  
👉 **[https://marylenh.github.io/Ressources_entreprises](https://marylenh.github.io/Ressources_entreprises)**

---

## 📚 Contenu de la formation

| Module | Sujet |
|--------|-------|
| 01 | Introduction aux statistiques d'entreprises |
| 02 | Unités statistiques et concepts clés (NAF, NACE...) |
| 03 | Sources françaises — L'INSEE (ESANE, SIRENE) |
| 04 | Sources européennes — Eurostat (SBS/EBS) |
| 05 | Open Data & data.gouv.fr |
| 06 | Analyse de données avec R (tidyverse, ggplot2) |
| 07 | Analyse de données avec Python (pandas, plotly) |
| — | Cas pratiques (4 études de cas approfondies) |
| — | Exercices progressifs (3 niveaux) |
| — | Ressources, glossaire et bibliographie |

---

## 🗂️ Structure du dépôt

```
Ressources_entreprises/
├── _quarto.yml                    # Configuration Quarto
├── index.qmd                      # Page d'accueil
├── styles.scss                    # Styles personnalisés
├── README.md                      # Ce fichier
│
├── chapters/                      # Chapitres de cours
│   ├── 01-introduction.qmd
│   ├── 02-concepts.qmd
│   ├── 03-sources-francaises.qmd
│   ├── 04-sources-europeennes.qmd
│   ├── 05-opendata.qmd
│   ├── 06-analyse-r.qmd
│   └── 07-analyse-python.qmd
│
├── case-studies/                  # Cas pratiques
│   └── index.qmd
│
├── exercises/                     # Exercices progressifs
│   └── index.qmd
│
├── resources/                     # Ressources et glossaire
│   └── index.qmd
│
├── data/                          # Données exemple (illustratives)
│   ├── esane_secteurs_2022_exemple.csv
│   ├── creations_defaillances_mensuelles_exemple.csv
│   ├── sbs_eurostat_exemple.csv
│   └── README.md
│
├── assets/                        # Ressources statiques
│   └── footer-scripts.html
│
└── .github/
    └── workflows/
        └── publish.yml            # Workflow GitHub Actions
```

---

## 🚀 Déploiement sur GitHub Pages

### Prérequis

1. **Quarto** installé localement (version ≥ 1.4) : [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/)
2. **R** (≥ 4.3) avec les packages : `tidyverse`, `knitr`, `jsonlite`, `scales`
3. **Python** (≥ 3.10) avec les packages : `pandas`, `numpy`, `matplotlib`, `plotly`, `requests`

### Déploiement automatique (recommandé)

Le site est automatiquement construit et déployé sur GitHub Pages à chaque `push` sur la branche `main`, grâce au workflow `.github/workflows/publish.yml`.

**Pour activer GitHub Pages dans votre dépôt :**

1. Allez dans **Settings** → **Pages**
2. Dans **Source**, sélectionnez **GitHub Actions**
3. Le prochain push sur `main` déclenchera le déploiement automatique

### Développement local

```bash
# Cloner le dépôt
git clone https://github.com/MaryleneH/Ressources_entreprises.git
cd Ressources_entreprises

# Installer les dépendances R (depuis R ou RStudio)
install.packages(c("tidyverse", "knitr", "jsonlite", "scales", "DT"))

# Installer les dépendances Python
pip install pandas numpy matplotlib plotly requests

# Prévisualiser le site en local
quarto preview

# Construire le site
quarto render
```

Le site construit sera disponible dans le dossier `_site/`.

---

## 📖 Sources officielles

Ce contenu s'appuie exclusivement sur des sources officielles vérifiées :

| Institution | Rôle | Site |
|-------------|------|------|
| **INSEE** | Statistiques nationales françaises | [insee.fr](https://www.insee.fr) |
| **Eurostat** | Statistiques européennes harmonisées | [ec.europa.eu/eurostat](https://ec.europa.eu/eurostat) |
| **data.gouv.fr** | Plateforme open data française | [data.gouv.fr](https://www.data.gouv.fr) |

> ⚠️ Les données numériques présentes dans ce site sont des **illustrations pédagogiques** basées sur les ordres de grandeur publiés par ces institutions. Pour des analyses précises, téléchargez toujours les données officielles directement depuis les sources indiquées.

---

## ⚖️ Licence

Le contenu pédagogique de ce site est mis à disposition sous licence [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

Vous êtes libre de partager et d'adapter ce contenu, à condition de citer la source.

---

## 🤝 Contribution

Les contributions sont les bienvenues ! Pour proposer des améliorations :

1. Ouvrez une [issue](https://github.com/MaryleneH/Ressources_entreprises/issues)
2. Forkez le dépôt et créez une branche
3. Soumettez une Pull Request

---

*Fait avec ❤️ et [Quarto](https://quarto.org)*
