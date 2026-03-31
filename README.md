# Coursera Capstone — IBM Data Science Professional Certification

This repository contains the capstone project for the **IBM Data Science Professional Certification** on Coursera.

## Project Overview

The main objective of this project is the **segmentation and clustering of the 14 municipalities** that make up the **San Salvador Metropolitan Area (AMSS — Área Metropolitana de San Salvador)**, El Salvador. Using unsupervised machine learning techniques, the project identifies patterns and trends among the municipalities to support better decision-making by authorities, businesses, and individuals.

## Problem Statement

The San Salvador Metropolitan Area is a highly populated and complex region from social, economic, and geographic perspectives. Its 14 municipalities have distinct characteristics and needs, which makes it difficult for authorities to identify common issues and allocate resources effectively. This project addresses that challenge by grouping municipalities based on venue data and population statistics.

## Data Sources

- **Foursquare API** — venue and location data (commercial establishments, tourist attractions, restaurants, etc.) within a 1,000-meter radius of each municipality's geographic center.
- **Nominatim / geopy** — geographic coordinates for each municipality.
- **Wikipedia** — list of the 14 municipalities in the AMSS ([Área metropolitana de San Salvador](https://es.wikipedia.org/wiki/Área_metropolitana_de_San_Salvador)).

## Methodology

- Data collection, cleaning, and preprocessing.
- Exploratory data analysis — most common venue categories per municipality.
- **K-Means clustering** applied in three ways:
  1. Municipalities grouped by type and count of nearby venues.
  2. Municipalities grouped by population size.
  3. Individual venues grouped by geographic proximity.

## Key Results

- **Cluster 0**: Municipalities dominated by restaurants, cafés, supermarkets, and bars — generally the most populated areas of the AMSS.
- **Cluster 1**: Municipalities on the outskirts of the city, featuring typical/Latin American food venues and open-air spaces.
- **Cluster 2**: Ilopango — a municipality near a lake and an airport, with restaurants as the predominant venue category.

Population-based clustering identified San Salvador and Soyapango as the most populous and economically active municipalities, while Antiguo Cuscatlán — despite being one of the least populous — holds the highest GDP in the country.

## Repository Contents

| File | Description |
|---|---|
| `Coursera Capstone project.ipynb` | Initial notebook — project setup and base code |
| `San_Salvador_municipios.ipynb` | Data collection and exploratory analysis |
| `San_Salvador_municipios (1)FINAL.ipynb` | Final version of the analysis notebook |
| `Informe_Final_Final.ipynb` | Final project report with full methodology, results, and conclusions |
| `Toronto-vecindarios.ipynb` | Practice notebook — neighbourhood segmentation in Toronto, Canada |
| `imagenes/` | Supporting images used in the notebooks |

## Technologies & Libraries

- **Python 3**
- `pandas`, `numpy` — data manipulation
- `geopy` / `Nominatim` — geocoding
- `folium` — interactive maps
- `scikit-learn` — K-Means clustering
- `matplotlib`, `seaborn` — data visualisation
- Foursquare Places API

## Conclusions

This project provides a general overview of how venues and businesses are distributed across the municipalities of the San Salvador Metropolitan Area and demonstrates how K-Means clustering can reveal meaningful geographic and economic patterns. Results can inform government entities, companies, and individuals when making decisions about opening a business or implementing commercial or tourism public policies in the region.
