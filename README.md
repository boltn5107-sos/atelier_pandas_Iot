# Atelier Pandas

<p align="center">
  <a href="https://www.python.org"><img src="assets/icons/python-original.svg" alt="Python" width="32" height="32"></a>&nbsp;&nbsp;
  <a href="https://pandas.pydata.org"><img src="assets/icons/pandas-original.svg" alt="Pandas" width="32" height="32"></a>&nbsp;&nbsp;
  <a href="https://numpy.org"><img src="assets/icons/numpy-original.svg" alt="NumPy" width="32" height="32"></a>&nbsp;&nbsp;
  <a href="https://jupyter.org"><img src="assets/icons/jupyter-original.svg" alt="Jupyter" width="32" height="32"></a>
</p>

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
