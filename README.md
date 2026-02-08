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

The repository is organized into **six top-level folders**, one per location:

- **Colombia/**
- **Bogotá/**
- **Spain/**
- **Barcelona/**
- **Germany/**
- **Munich/**

These locations include **three countries** and, for each one, **a major city**, in order to capture both rural and urban environments.

---

## Per-location folder contents

Inside each location folder, there are **100 subfolders** (one per experiment instance), e.g.:

Spain/
exp_001/
exp_002/
...
exp_100/
results_Spain.xlsx


### Per-experiment contents

Each `exp_XXX/` folder contains Folium-generated HTML files:

- `osm_raw.html` — raw graph downloaded from OpenStreetMap  
- `graph_simplified.html` — simplified graph used as the optimization input  
- One HTML file per studied architecture/strategy, e.g.:
  - `ptp.html`
  - `bpon_heuristic.html`
  - `upon_heuristic.html`
  - `bpon_milp.html`
  - `upon_milp.html`

(Exact filenames may vary slightly across folders.)

### Per-location Excel summary

Each location folder includes one Excel file (e.g., `results_Spain.xlsx`) containing the **aggregated results of the 100 experiments** in that location.

---

## Global aggregated results

At the repository root, an Excel file aggregates **all experiments across the six locations**, including:
- combined tables with all runs,
- summary statistics,
- plots used in the statistical analysis reported in the paper.

> Paper reference: **[ADD CITATION / DOI / ARXIV LINK HERE]**

---

## Notes

- This repository is intended as a **results dump** (no benchmark scripts or comparative evaluation code is included here).
- The detailed methodology and analysis are described in the associated paper [Insert reference when published].
