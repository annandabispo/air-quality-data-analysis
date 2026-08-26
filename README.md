[🇧🇷 Versão em Português](README.pt-BR.md)

#  Air Quality Data Analysis

Exploratory Data Analysis (EDA) of air quality measurements collected in an urban area of **Milan, Italy**, between March 2004 and February 2005.

This project explores how **climatic and temporal factors are associated with atmospheric pollutant concentrations**, focusing on CO, NOx and NO₂.

The analysis was developed in Python using data cleaning, descriptive statistics, data visualization and hypothesis-driven exploratory analysis.

---

##  Project Objective

The main goal of this project is to investigate patterns in urban air pollution and explore possible relationships between pollutant concentrations, environmental conditions and temporal factors.

The analysis focuses on:

- `CO(GT)` — Carbon Monoxide
- `NOx(GT)` — Nitrogen Oxides
- `NO2(GT)` — Nitrogen Dioxide
- Temperature
- Relative and absolute humidity
- Time of day
- PT08 sensor responses

---

##  Research Questions

The exploratory analysis was structured around six main hypotheses:

**H1 — Temperature and pollution**  
Are lower temperatures associated with higher pollutant concentrations?

**H2 — Humidity and pollution**  
Are higher humidity levels associated with higher concentrations of atmospheric pollutants?

**H3 — Cold periods and nitrogen oxides**  
Do colder periods present higher concentrations of NOx and NO₂?

**H4 — Daily patterns**  
Do CO, NOx and NO₂ concentrations vary throughout the day?

**H5 — Relationship between NOx and NO₂**  
Do NOx and NO₂ exhibit similar temporal behavior?

**H6 — PT08 sensors and reference measurements**  
Do PT08 sensor responses follow patterns similar to the corresponding reference measurements?

---

##  Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Google Colab

---

##  Data Preparation

Before performing the exploratory analysis, the dataset was inspected and cleaned.

The main preprocessing steps included:

- identification and treatment of missing or invalid measurements;
- replacement of the `-200` code used for unavailable measurements with `NaN`;
- combination of date and time information into a single `Datetime` variable;
- inspection of descriptive statistics and distributions;
- identification of outliers;
- preparation of temporal and environmental variables for further analysis.

The original dataset was preserved, while auxiliary DataFrames were created when transformations were required for specific analyses.

---

##  Exploratory Analysis

The project combines different approaches to understand the behavior of atmospheric pollutants:

- descriptive statistics;
- distribution analysis;
- outlier detection;
- comparison across temperature ranges;
- comparison across humidity ranges;
- analysis of cold and warmer periods;
- hourly pollution patterns;
- monthly temporal behavior;
- comparison between reference measurements and PT08 sensor responses.

---

## Key Findings

###  Lower temperatures were associated with higher NOx and NO₂ levels

One of the clearest patterns observed in the analysis was the relationship between temperature and nitrogen oxides.

NOx concentrations progressively decreased across higher temperature ranges, while NO₂ also showed higher average concentrations during colder conditions.

When the dataset was divided into colder and warmer periods, **both NOx and NO₂ presented higher average concentrations during colder periods**.

---

###  Humidity showed different relationships across pollutants

The relationship between relative humidity and pollution was not consistent across all pollutants.

NOx concentrations increased across higher humidity ranges, while CO showed relatively small variations and NO₂ followed a different pattern.

This suggests that environmental conditions may interact differently with each pollutant.

---

###  Pollution levels showed clear hourly patterns

CO, NOx and NO₂ concentrations varied considerably throughout the 24-hour cycle.

The analysis identified lower concentrations during parts of the early morning, followed by increases during the morning and another noticeable rise during the late afternoon and early evening.

These patterns indicate a clear temporal component in urban air pollution levels.

---

###  NOx and NO₂ showed partially similar temporal behavior

NOx and NO₂ exhibited similar trends during several periods of the analysis, including higher concentrations under colder conditions and comparable variations throughout the day.

However, differences in the timing and intensity of their peaks indicate that their behavior is **related but not identical**.

---

###  PT08 sensors did not consistently follow reference measurements

The comparison between selected PT08 sensors and their corresponding reference measurements revealed periods of both similarity and divergence.

The sensor responses did not consistently reproduce the temporal behavior observed in the reference measurements, suggesting an interesting opportunity for further investigation into **sensor calibration and performance**.

---

##  Hypothesis Summary

| Hypothesis | Result |
|---|---|
| H1 — Temperature and pollution | 🟡 Partially supported |
| H2 — Humidity and pollution | 🟡 Partially supported |
| H3 — Cold periods and NOx/NO₂ | 🟢 Supported |
| H4 — Daily pollution patterns | 🟢 Supported |
| H5 — NOx and NO₂ behavior | 🟡 Partially supported |
| H6 — PT08 sensor behavior | 🔴 Not supported by the visual analysis |

> The results represent associations observed in the dataset and should not be interpreted as evidence of causality.

---

## Conclusion

The exploratory analysis revealed meaningful relationships between **environmental conditions, temporal patterns and atmospheric pollutant concentrations**.

Among the most relevant findings were the higher average concentrations of NOx and NO₂ during colder periods and the clear variation of pollutant levels throughout the day.

The project also demonstrated that different pollutants respond differently to environmental conditions and highlighted potential differences between reference measurements and sensor responses.

Overall, this analysis demonstrates how exploratory data analysis can transform environmental measurements into meaningful insights, while also generating new questions for further investigation.

---

## Future Improvements

Possible next steps for this project include:

- Developing Machine Learning models to predict pollutant concentrations;
- Investigating seasonal patterns in greater depth;
- Detecting anomalous pollution events;
- Evaluating PT08 sensor calibration and performance;
- Creating an interactive air quality dashboard;
- Incorporating additional environmental or urban variables.

---

##  Notebook

The complete analysis is available in:

**`Analise_Qualidade_Ar.ipynb`**

> **Note:** The complete exploratory analysis inside the notebook is documented in Portuguese.

---

## Author

**Annanda Bispo**  
Computer Engineering — UFRN

Interested in **Data Science, Artificial Intelligence and Data Analytics**.
