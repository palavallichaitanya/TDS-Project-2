# Automated Data Analysis and Visualization

## Overview

This project focuses on the development of an advanced Python-based system engineered to automate data analysis, visualization, and insight narration from any given dataset. By harnessing the capabilities of a Large Language Model (LLM) in conjunction with state-of-the-art data processing and visualization techniques, the system produces comprehensive Markdown reports enhanced with high-quality visual representations. Designed for versatility, it ensures compatibility with a wide range of CSV datasets, catering to diverse analytical requirements.
---

## Features
### 1. Comprehensive Automated Analysis
- Performs detailed summary statistics, identifies missing values, and detects anomalies with precision.
- Conducts sophisticated correlation studies and clustering analyses to reveal latent patterns in data.
- Utilizes the LLM to provide advanced insights, suggest novel analytical techniques, and recommend methodological improvements.

### 2. Dynamic Visualization Generation
- Automatically generates 1–3 visually appealing charts in PNG format tailored to the dataset.
- Leverages a diverse array of visualizations, including heatmaps and bar charts, to suit the dataset’s attributes and analytical outcomes.

### 3. Narrative and Insight Generation
- Engages the LLM to craft detailed narratives encompassing dataset descriptions, analysis methodologies, significant findings, and their broader implications.
- Produces a cohesive Markdown report (`README.md`) integrating narratives with visual elements for seamless comprehension.

### 4. Efficient LLM Resource Utilization
- Reduces reliance on direct dataset transfers by preprocessing and summarizing data before querying the LLM.
- Optimizes token consumption while ensuring analytical depth and precision.

### 5. Universal CSV Dataset Compatibility
- Adapts dynamically to datasets of varying column types, distributions, and complexities, ensuring robust and scalable performance.

### 6. Self-Contained and Independent Execution
- Operates as a standalone script (`autolysis.py`) requiring no external dependencies beyond standard Python libraries.

### 7. Ease of Use and Integration
- Simplifies execution via the `uv` CLI tool with a single command for end-to-end functionality:
  ```bash
  uv run autolysis.py dataset.csv
  ```
---

## Datasets Analyzed

The tool has been applied to several datasets to demonstrate its capabilities:

1. **Goodreads Dataset**:
   - Analyzes books, ratings, authors, and genres.
   - Provides insights into book ratings, the popularity of genres, and author profiles.

2. **Media Dataset**:
   - Examines media views, ratings, and genres.
   - Delivers insights into media consumption patterns, popularity, and audience preferences.

3. **Happiness Dataset**:
   - Evaluates happiness scores based on income, education, and social support by country.
   - Offers insights into global happiness trends and factors influencing well-being.

---

## How to Use

### 1. Upload Dataset
To begin using the tool, simply upload your dataset. The system supports a variety of formats, including CSV, Excel, and JSON. 

### 2. Data Analysis
Once the dataset is uploaded, the tool will automatically load and begin the analysis. The following processes will be carried out:
   - **Data Cleaning**: The tool checks for missing values, duplicates, and other inconsistencies.
   - **Statistical Summaries**: The system generates summary statistics for all numerical and categorical columns, including mean, median, mode, standard deviation, and more.
   - **Correlation Analysis**: The tool calculates correlation coefficients to reveal relationships between numerical variables.
   - **Data Visualizations**: Visualizations such as distribution plots, box plots, and heatmaps are generated for a better understanding of the data.

### 3. Insights & Reporting
After the analysis is complete, the tool will generate:
   - **Statistical Summary Report**: A detailed summary of all calculated statistics.
   - **Visualizations**: All generated charts are saved as PNG files for easy sharing and inclusion in reports.
   - **Narrative Insights**: Using OpenAI’s models, the tool produces a written analysis summarizing key findings, trends, and insights from the data.

### 4. Save and Export
Once the analysis is complete, you can:
   - Download the statistical summary as a text or CSV file.
   - Download the generated visualizations as PNG files.
   - Export the generated narrative report.
## Technical Notes
- **Optimized LLM Utilization:**
  - Employs multiple queries to the LLM for detailed analyses and visualization recommendations.
  - Integrates OpenAI’s function-calling API for enhanced precision.

- **Environment Configuration:**
  - Requires the `AIPROXY_TOKEN` environment variable for LLM authentication.

- **Visualization Tools:**
  - Utilizes Seaborn and Matplotlib to create compelling and insightful visualizations.

## Deliverables
1. **Core Python Script:**
   - `autolysis.py`: A standalone script encapsulating all functionalities.
2. **Generated Output Files:**
   - Separate directories for each dataset (e.g., `goodreads/`, `happiness/`, `media/`) containing:
     - `README.md`: The comprehensive Markdown report.
     - `*.png`: Visualization files in PNG format.

## Licensing
This project is licensed under the MIT License. For details, refer to the LICENSE file in the repository.

---

This project aims to exemplify the seamless integration of advanced analytical techniques and LLM capabilities, offering both technical rigor and practical utility. Best wishes for your journey into automated data analysis and visualization!
