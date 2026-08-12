# Atelier Pandas

[![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org)
[![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?style=flat-square&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![NumPy](https://img.shields.io/badge/NumPy-2.x-013243?style=flat-square&logo=numpy&logoColor=white)](https://numpy.org)
[![Jupyter](https://img.shields.io/badge/Jupyter_Notebook-F37626?style=flat-square&logo=jupyter&logoColor=white)](https://jupyter.org)
[![License](https://img.shields.io/badge/Licence-MIT-2ea44f?style=flat-square)](LICENSE)

Atelier pratique de préparation et d'analyse de données avec **Pandas**.

## Contexte

Une entreprise possède plusieurs bâtiments équipés de capteurs **IoT**. Chaque capteur collecte
régulièrement la température, l'humidité, la pression, la consommation énergétique, l'état du
capteur, le bâtiment, ainsi que la date et l'heure de la mesure. Les données doivent être préparées
et analysées avant d'être transmises à un futur système de **Machine Learning** chargé de détecter
des situations anormales.

## Structure du projet

```
atelier_pandas_iot/
│
├── data/                                # Données brutes
│   └── mesures_capteurs.csv
│
├── notebooks/                           # Notebook d'analyse
│   └── atelier_pandas_iot.ipynb
│
└── exports/                             # Données nettoyées (généré)
    ├── donnees_nettoyees.csv
    └── donnees_nettoyees.json
```

## Déroulé de l'atelier

| Partie | Thème |
|--------|-------|
| 1  | Series |
| 2  | DataFrame |
| 3  | Exploration |
| 4  | Sélection |
| 5  | Manipulation des colonnes |
| 6  | Filtrage |
| 7  | Tri |
| 8  | Analyse (`groupby`) |
| 9  | Gestion des valeurs manquantes |
| 10 | Gestion des doublons |
| 11 | Statistiques descriptives |
| 12 | Exportation |
| 13 | Bonus |

## Installation

```bash
python -m venv .venv
source .venv/bin/activate          # Windows : .venv\Scripts\activate
python -m pip install pandas numpy jupyter
```

## Utilisation

```bash
jupyter notebook notebooks/atelier_pandas_iot.ipynb
```

Le notebook charge les mesures depuis `data/mesures_capteurs.csv` et écrit les données nettoyées
dans `exports/` à l'issue de l'atelier.
