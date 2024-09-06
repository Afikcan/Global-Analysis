# Global Analysis: Faith, Education, and Prosperity

## Table of Contents
- [Introduction](#introduction)
- [Research Questions](#research-questions)
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

This project investigates the intersection of religiousness, educational attainment, and economic welfare (Human Development Index - HDI) across five countries: **Norway**, **Australia**, **Saudi Arabia**, **India**, and **Afghanistan**. By analyzing global data from 1990 to 2010, this study aims to uncover patterns between non-religiosity, education levels, and economic development, providing insights into how these factors interplay across distinct cultural and economic environments.

For a more detailed breakdown of the methodology, statistical models, and findings, please refer to the [project paper](Exploring_the_Intersection_of_Religion__Education__and_Economic_Welfare__A_Global_Analysis.pdf) written for the class project.

## Research Questions

This study is driven by the following research questions:

1. **How does non-religiosity relate to educational attainment and HDI in countries with varying levels of religious adherence?**
2. **What is the correlation between levels of education and economic welfare in secular and religious societies?**
3. **How do the interactions between religious adherence, education, and economic development differ across regions like Europe, the Middle East, and South Asia?**

These research questions aim to explore the complex relationships between religion, education, and economic welfare, with a specific focus on whether secularism is a factor in boosting educational and economic outcomes.

## Dataset

The dataset comprises global data on religious adherence, educational attainment, and HDI across five countries from 1990 to 2010. Key variables include:

- **Religiousness**: Levels of religious adherence in each country.
- **Educational Attainment**: The percentage of the population that has achieved various levels of education.
- **Economic Welfare (HDI)**: A composite measure that includes life expectancy, education, and per capita income indicators.

### Key Features

- **Countries**: Norway, Australia, Saudi Arabia, India, Afghanistan
- **Time Period**: 1990–2010
- **Variables**:
  - Religious adherence
  - Educational attainment
  - HDI (Human Development Index)

### Data Sources

The dataset was sourced from multiple global data repositories, including:
- **UN Data**: The United Nations Development Program (UNDP) and various global reports.
- **World Bank**: Key economic and social indicators, including GDP and literacy rates.

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

The study employs various statistical techniques to explore the relationships between religiousness, educational attainment, and economic welfare:

### Data Preprocessing

The dataset was cleaned and standardized to account for missing values, inconsistent measurements across countries, and outliers. Standardization ensures that the various scales of data (e.g., education percentages, HDI scores) are suitable for further statistical analysis.

### Dimension Reduction

To handle the complexity of the dataset and reduce redundancy, **Principal Component Analysis (PCA)** was used to reduce the number of dimensions. This allowed for capturing the most critical aspects of the dataset while improving the efficiency and interpretability of the analysis.

### Correlation Analysis

**Pearson correlation coefficients** were computed to determine the strength of relationships between variables such as non-religiosity, education, and HDI. This analysis revealed strong positive correlations between educational attainment and HDI in countries like **Norway** and **Australia**, where religious adherence was relatively low. Meanwhile, countries like **Saudi Arabia**, **India**, and **Afghanistan** exhibited more complex interactions between religious adherence and economic outcomes.

### Regression Models

The study also uses **Multiple Linear Regression** models to predict HDI based on religious adherence and educational attainment. The regression models provided insights into how these variables interact to influence a country's economic welfare. For instance:

- **Secular countries** like Norway showed a stronger positive impact of education on HDI, with religiousness having minimal influence.
- **Religious countries**, such as Afghanistan and Saudi Arabia, revealed that religious adherence sometimes acted as a limiting factor in improving educational attainment and HDI.

## Results

The study yielded several significant findings:

- **Norway and Australia**: Secularism appears to promote educational attainment, which in turn boosts HDI.
- **Saudi Arabia**: While education is a key driver of HDI, the role of religiousness in shaping socio-economic outcomes is more nuanced and context-dependent.
- **India and Afghanistan**: In these countries, higher levels of religious adherence were generally associated with lower educational attainment and lower HDI, though the relationship is influenced by other socio-political factors.

These findings suggest that while education is universally associated with higher economic welfare, the role of religious adherence varies significantly across different socio-cultural contexts.

## Conclusion

This project demonstrates that educational attainment consistently correlates with higher economic welfare, as measured by HDI, but religious adherence can either complement or complicate this relationship depending on the country's cultural and socio-political context. Secular nations tend to benefit more from education in terms of HDI growth, whereas religious nations show more complex patterns.
