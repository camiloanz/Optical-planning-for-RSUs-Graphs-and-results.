# Optical-planning-for-RSUs-Graphs-and-results.
Repository of experimental results on optical access-network planning for RSU interconnection, including graph layouts and raw obtained data for 600 experiments.
# RSU Optical Planning – Raw Results Dataset

This repository contains **raw experimental outputs** for optical access-network planning aimed at **RSU interconnection**. It includes results for:
- **Point-to-Point (PtP)**
- **Balanced PON heuristic (BPON heuristic)**
- **Unbalanced PON heuristic (UPON heuristic)**
- **BPON MILP**
- **UPON MILP**

For each experiment, the repository provides **Folium (HTML) visualizations** of the input graphs and the resulting deployment layouts, as well as **Excel files** with aggregated numerical results.

---

## Repository structure

The repository is organized into **six top-level folders (zip files)**, one per location:

- **Colombia/**
- **Bogotá/**
- **Spain/**
- **Barcelona/**
- **Germany/**
- **Munich/**

These locations include **three countries** and, for each one, **a major city**, in order to capture both rural and urban environments.

---

## Per-location folder contents

Inside each location folder, there are **100 subfolders** (one per experiment instance), and an Excel fil with numeric results e.g.:

Spain/
1/
2/
...
100/
results_Spain.xlsx

Bogotá's folder has two parts because of its size.

### Per-experiment contents

Each subfolder contains Folium-generated HTML files:

- `Raw_graph_place_test.html` — raw graph downloaded from OpenStreetMap  
- `Simple_graph_place_test.html` — simplified graph used as the optimization input  
- One HTML file per studied architecture/strategy, e.g.:
  - `PtP_place_test.html` = Point to Point
  - `BPON_HEU_place_test.html` = BPON heuristic
  - `UPON_HEU_place_test.html` = UPON heuristic
  - `BPON_COST_place_test.html` = BPON MILP cost optimization
  - `UPON_COST_place_test.html` = UPON MILP cost optimization

Additionally, a .pkl (pickled NetworkX graph) file is provided for each input graph to support reproducibility.
  - `Simple_graph_place_test.pkl`

### Per-location Excel summary

Each location folder includes one Excel file (e.g., `results_Spain.xlsx`) containing the **aggregated results of the 100 experiments** in that location. It includes all input graph metrics, and results measurements in separated sheets (e.g., Cost, fiber, splitters, etc)

---

## Global aggregated results

At the repository root, an Excel file aggregates **all experiments across the six locations**.Histograms (Histograms.zip) and Spearman´s correlation analysis of savings (Correlations.zip) are also included.

> Paper reference: **[ADD CITATION / DOI / LINK HERE]**

---

## Notes

- This repository is intended as a **results dump** (no benchmark scripts or comparative evaluation code is included here).
- The detailed methodology and analysis are described in the associated paper [Insert reference when published].
