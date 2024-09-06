# Global Analysis: Faith, Education, and Prosperity

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Usage](#usage)
- [Approach](#approach)
  - [Data Preprocessing](#data-preprocessing)
  - [Dimension Reduction](#dimension-reduction)
  - [Correlation Analysis](#correlation-analysis)
  - [Regression Models](#regression-models)
- [Results](#results)
- [Conclusion](#conclusion)

## Introduction

This project explores the intersection of religiousness, educational attainment, and economic welfare (Human Development Index - HDI) across five countries: **Norway**, **Australia**, **Saudi Arabia**, **India**, and **Afghanistan**. By analyzing global data from 1990 to 2010, the project investigates how non-religiosity, education levels, and economic welfare correlate across these culturally distinct nations.

For more comprehensive details on the methodology, statistical analysis, and insights, you can refer to the [project paper](Exploring_the_Intersection_of_Religion__Education__and_Economic_Welfare__A_Global_Analysis.pdf) written for my class.

## Dataset

The dataset comprises key socio-economic indicators over a 20-year period for five countries, exploring the links between:

- **Religiousness**: Levels of religious adherence in each country.
- **Educational Attainment**: Percentage of the population with varying levels of education.
- **Economic Welfare (HDI)**: A composite measure including life expectancy, education, and per capita income indicators.

### Key Features

- **Countries**: Norway, Australia, Saudi Arabia, India, Afghanistan
- **Time Period**: 1990 to 2010
- **Variables**:
  - Religiousness: Religious adherence levels.
  - Educational Attainment: Percent of the population with various education levels.
  - HDI: A composite index of human development.

### Data Sources

- **UN Data**: The United Nations Development Program (UNDP) and various global reports.
- **World Bank**: Economic and social indicators, including GDP and literacy rates.

## Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/Afikcan/Global-Analysis.git
    cd Global-Analysis
    ```

2. Unzip the dataset:
    - The data is in `data.zip`. Unzip it in the root directory.

3. Open the Jupyter notebook:
    ```bash
    jupyter notebook main.ipynb
    ```

4. Run the notebook to:
    - Perform dimensionality reduction using PCA.
    - Conduct correlation and regression analysis.
    - Visualize the relationships between religiousness, education, and HDI.

## Approach

The project follows a structured methodology to analyze the relationships between the variables:

### Data Preprocessing

The data was cleaned to handle missing values and discrepancies across countries and years. The dataset was scaled to standardize variables and make them suitable for correlation and regression analysis. Outliers were identified and addressed to ensure accurate model performance.

### Dimension Reduction

**Principal Component Analysis (PCA)** was used to reduce the dimensionality of the dataset, allowing the most important features to be retained while removing redundancy. This technique was especially useful for high-dimensional data, improving computational efficiency and interpretability.

### Correlation Analysis

Correlation coefficients were calculated to explore the relationships between non-religiosity, educational attainment, and HDI. The analysis revealed significant patterns:

- Countries like **Norway** and **Australia** exhibit strong positive correlations between education and HDI, with low levels of religious adherence.
- **Saudi Arabia**, **India**, and **Afghanistan** showed more complex relationships, where religious adherence played a varying role in the socio-economic outcomes.

### Regression Models

**Multiple Linear Regression** models were built to predict HDI based on educational attainment and religious adherence. The models highlighted how these factors interacted differently across countries:

- In **secular countries** like Norway, educational attainment had a stronger impact on HDI.
- In **religiously inclined countries**, such as Afghanistan, religious adherence influenced both educational attainment and HDI, but the effects varied across time and regions.

## Results

The analysis uncovered several important findings regarding the relationship between education, religion, and economic welfare:

- **Norway and Australia**: These countries exhibit a strong positive correlation between higher educational attainment and higher HDI, with low levels of religious adherence.
- **Saudi Arabia**: Education is a key driver of HDI, but religiousness plays a complex role in societal outcomes.
- **India and Afghanistan**: Higher levels of religiousness often correlate with lower educational attainment and lower HDI, but the relationships are nuanced and depend on other socio-political factors.

The results indicate that while education tends to drive economic welfare, religious adherence can either complement or conflict with educational attainment depending on the cultural and socio-political context.

## Conclusion

This project provides a comparative analysis of five countries, illustrating how different socio-economic, religious, and educational dynamics shape human development. The study shows that educational attainment is a consistent driver of HDI, but religious adherence plays a more variable role, depending on the country and cultural context.

For a detailed explanation of the methods, statistical models, and in-depth insights, please refer to the [project paper](Exploring_the_Intersection_of_Religion__Education__and_Economic_Welfare__A_Global_Analysis.pdf).
