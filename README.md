# Brazilian Real Estate Analysis

## Overview

This project analyzes Brazilian real estate data to investigate housing characteristics, relationships between variables, property prices, and location effects.

The analysis applies practical data-science methods including data understanding, visualization, correlation analysis, and price-per-square-meter analysis.

The project is based on a Brazilian real estate dataset provided through WorldQuant University course materials. The original course module uses a Mexican real estate dataset; this project independently applies the same core data-science concepts to the provided Brazilian dataset.

## Research Questions

The analysis investigates:

1. What are the main characteristics of the Brazilian real estate data?
2. How are housing characteristics and property prices distributed?
3. What relationships exist between property characteristics and price?
4. How does price per square meter vary across locations?

## Data

The datasets were provided through the WorldQuant University Applied Data Science Lab course materials.

The original course module, "Hands-on Data Science in the Mexican Real Estate Market," uses a Mexican real estate dataset. This project uses the provided Brazilian dataset instead and conducts the analysis independently.

The original source files are kept locally and are not included in this repository.

## Methodology

The analysis is organized into four notebooks:

### 01. Data Understanding

Examines the structure, variables, data types, missing values, and data quality of the Brazilian real estate datasets.

### 02. Housing Data Visualization

Uses descriptive statistics and visualizations to examine housing characteristics and property-price distributions.

### 03. Correlation and Relationships

Investigates relationships between numerical variables, with particular attention to relationships involving property price.

### 04. Price per Square Meter and Location

Calculates price per square meter and examines how property values vary across available geographic or location variables.

## Notebooks

| Notebook                                       | Purpose                                                         |
| ---------------------------------------------- | --------------------------------------------------------------- |
| `01_data_understanding.ipynb`                  | Understand the datasets and establish the analytical population |
| `02_housing_data_visualization.ipynb`          | Explore housing characteristics and distributions               |
| `03_correlation_and_relationships.ipynb`       | Analyze correlations and variable relationships                 |
| `04_price_per_square_meter_and_location.ipynb` | Analyze price per square meter and location effects             |

## Project Structure

```text
brazil-real-estate-analysis/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_housing_data_visualization.ipynb
│   ├── 03_correlation_and_relationships.ipynb
│   └── 04_price_per_square_meter_and_location.ipynb
├── reports/
│   └── figures/
├── docs/
│   └── data_dictionary.md
├── .gitignore
├── .python-version
├── pyproject.toml
├── uv.lock
└── README.md
```

## Tools

- Python
- pandas
- NumPy
- Matplotlib
- Jupyter
- uv

## Attribution

This project was developed independently using skills from the WorldQuant University Applied Data Science Lab.

The Brazilian real estate dataset used in this project was provided through the WorldQuant University course materials. The original course module uses a Mexican real estate dataset; this project applies the same core data-science concepts to the provided Brazilian dataset.

## Reproducibility

The project environment is managed with `uv`.

Create the environment and install the locked dependencies with:

```bash
uv sync
```

The source datasets are not included in the repository. Place the provided Brazilian datasets in:

```bash
data/raw/
```

The notebooks document the analytical workflow from source data through exploratory analysis.

## Status

In progress.

## Author

**Nkululeko Cyril Cele**
