# 📁 powerbi

Le projet Power BI **AHD Automobiles** au format **PBIP**, lisible et versionnable dans Git.

| Élément | Contenu |
|---|---|
| [`AHD Automobiles.pbip`](AHD%20Automobiles.pbip) | le fichier à ouvrir dans Power BI Desktop |
| [`AHD Automobiles.Report/`](AHD%20Automobiles.Report) | le rapport au format **PBIR** : 7 pages, 392 visuels, thème et images |
| [`AHD Automobiles.SemanticModel/`](AHD%20Automobiles.SemanticModel) | le modèle sémantique au format **TMDL** : 13 tables, 11 relations, 207 mesures |

## 🚀 Ouvrir le projet

1. Restaurez une base **`PrestigeCars`** sur votre instance **SQL Server**.
2. Ouvrez `AHD Automobiles.pbip` dans **Power BI Desktop**.
3. Dans **Transformer les données**, réglez les paramètres **`Serveur`** (par défaut `localhost`) et **`Base`** (par défaut `PrestigeCars`).
4. Cliquez sur **Actualiser** : les 7 pages se remplissent.

## 🔎 Où lire quoi

| Pour lire | Ouvrez |
|---|---|
| les tables et leurs colonnes | `AHD Automobiles.SemanticModel/definition/tables/` |
| les relations | `AHD Automobiles.SemanticModel/definition/relationships.tmdl` |
| les 207 mesures DAX | `AHD Automobiles.SemanticModel/definition/tables/Metrics.tmdl` |
| les paramètres de connexion | `AHD Automobiles.SemanticModel/definition/expressions.tmdl` |
| les pages et leurs visuels | `AHD Automobiles.Report/definition/pages/` |

Ce dossier **ne contient aucune donnée** : le cache local de Power BI est exclu par le `.gitignore`, et les données sont lues dans SQL Server à l'actualisation.

[⬅️ Retour au README principal](../README.md)
