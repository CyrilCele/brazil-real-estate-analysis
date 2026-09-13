# Brazilian Real Estate Analysis

## Overview

This project analyzes Brazilian real estate data to investigate housing characteristics, relationships between variables, property prices, and location effects.

The analysis applies practical data-science methods including data understanding, data cleaning, visualization, correlation analysis, and price-per-square-meter analysis.

The project uses a Brazilian real estate dataset provided through WorldQuant University course materials. The original course module uses a Mexican real estate dataset; this project independently applies the same core data-science concepts to the provided Brazilian dataset.

## Research Question

**How are property prices in the Brazilian real estate data associated with property size and location?**

The analysis investigates:

1. What are the main characteristics and data-quality issues in the Brazilian real estate datasets?
2. How are housing characteristics and property prices distributed?
3. What relationships exist between property characteristics and price?
4. How does price per square meter vary across locations?
5. How do property size and location relate to observed property prices?

## Data

The datasets were provided through the WorldQuant University Applied Data Science Lab course materials.

The original course module, "Hands-on Data Science in the Mexican Real Estate Market," uses a Mexican real estate dataset. This project uses the provided Brazilian dataset instead and conducts the analysis independently.

The project uses two Brazilian real estate datasets with information including:

- Property type
- State
- Region
- City or location information
- Latitude and longitude
- Property area
- Property price

The original source files are kept locally and are not included in this repository.

## Project Scope

This project focuses on data understanding, cleaning, integration, exploratory analysis, and relationships between property characteristics, prices, and location.

The cleaned and integrated dataset is structured so that it can be reused for future statistical or machine-learning analysis, including Linear Regression.

**Linear Regression is not developed or evaluated as part of this project.**

The purpose of the cleaning stage is to produce a consistent analytical dataset for this project and provide a reliable foundation for potential future modeling work.

## Data Engineering Approach

The project prioritizes retaining useful observations while addressing missing values and structural inconsistencies in a transparent way.

Rather than removing all observations containing missing values, the cleaning process evaluates missingness patterns and engineers appropriate replacements where sufficient contextual information is available.

Key transformations include:

- Standardizing data types and variable formats
- Converting property prices to a common currency
- Resolving structural differences between the two source datasets
- Handling missing property-area values using contextual grouped medians
- Deriving city information for records where city is not provided using geographic proximity to the available reference data
- Aligning the two datasets to a common schema
- Validating the resulting combined dataset before export

The resulting dataset is intended to preserve analytical coverage while maintaining a transparent record of the transformations applied.

## Methodology

The analysis is organized into four notebooks:

### 01. Data Understanding

Examines the structure, variables, data types, missing values, data-quality issues, and differences between the two Brazilian real estate datasets.

The notebook also cleans and standardizes the datasets, resolves structural differences, aligns their variables, combines them into a unified dataset, and exports the resulting cleaned data.

### 02. Housing Data Visualization

Uses descriptive statistics and visualizations to examine housing characteristics and property-price distributions.

### 03. Correlation and Relationships

Investigates relationships between numerical variables, with particular attention to relationships involving property price.

### 04. Price per Square Meter and Location

Calculates price per square meter and examines how property values vary across available geographic and location variables.

## Notebooks

| Notebook                                       | Purpose                                                                          |
| ---------------------------------------------- | -------------------------------------------------------------------------------- |
| `01_data_understanding.ipynb`                  | Understand, clean, standardize, and integrate the Brazilian real estate datasets |
| `02_housing_data_visualization.ipynb`          | Explore housing characteristics and property-price distributions                 |
| `03_correlation_and_relationships.ipynb`       | Analyze correlations and variable relationships                                  |
| `04_price_per_square_meter_and_location.ipynb` | Analyze price per square meter and location-related differences                  |

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
