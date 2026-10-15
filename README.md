# final_project_MATH2007
# Meteorite Landings Analysis

This project explores the locations and masses of meteorites in NASA’s public dataset.

## 🧠 Research Question

**Where are meteorites of masses of at least 1 kg located, how do counts change as the minimum mass increases, and in which countries were found the ten heaviest recorded meteorites ?**

## 📊 Dataset

- Source: https://data.nasa.gov/Space-Science/Meteorite-Landings/gh4g-9sfh
- File used: `data/meteorite_landings.csv`
- Map outlines: `data/world_countries.geojson` from Natural Earth

## 🧪 What the script does

- Automatically cleans the data; 
- Excludes missing masses and, for mapping, missing/invalid coordinates and questionable `(0, 0)`.
- Maps meteorites weighing at least 1 kg.
- Counts records at four mass thresholds.
- Plots the ten heaviest records with their countries.

## 📁 Output

Three charts and two CSV tables are saved in `outputs/`:

- `meteorite_locations.png`
- `mass_threshold_counts.png` and `.csv`
- `heaviest_meteorites.png` and `.csv`

## ▶️ How to run

Requires Python 3.11+, pandas, and Matplotlib. Run from the project folder with both `data/` files present:

```sh
python3 -m pip install -r requirements.txt
mkdir -p outputs
python3 analysis.py
```

Use the included data to reproduce the results.
