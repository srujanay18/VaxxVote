# VaxxVote
## Contents of the Repository
### Section 1: Software and Platform Section
## Software and Platform

**Software:** Google Colab and Jupyter Notebooks

**Add-on packages:**
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- scipy

**Platform:** Windows and Mac

## Map of the Documentation

```markdown VaxxVote/
├── DATA/
│ ├── final_datasets/
│ │ ├── merged_influenza_presidents_data.csv
│ │ └── merged_vaccination_presidents_data.csv
│ ├── original_datasets/
│ │ ├── Diphtheria tetanus toxoid and pertussis (DTP) vaccination coverage 2025-15-10 15-11 UTC (2).xlsx
│ │ ├── Measles vaccination coverage 2025-15-10 14-12 UTC.xlsx
│ │ ├── Rubella vaccination coverage 2025-20-10 09-42 UTC.xlsx
│ │ └── Influenza Vaccine Doses Distributed in the United States, By Season (1).csv
│ └── README.md
├── SCRIPTS/
│ ├── 1_cleaning.ipynb
│ ├── 2_exploratory_plots.ipynb
│ └── 3_model.ipynb
├── OUTPUT/
│ └── model_visualizations/
│ ├── f_Influenza Doses Administered Over Time by Political Party.png
│ ├── f_Vaccination Coverage Over Time by Political Party.png
│ ├── t_OLS regression results influenza.png
│ └── t_OLS regression results vaccinations.png
├── LICENSE
└── README.md```


## Instructions for Reproducing the Results

1. **Clone the repository:**
   ```bash
   git clone https://github.com/srujanay18/VaxxVote.git
   cd VaxxVote
   ```

2. **Install required packages:**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn scipy 
   ```

3. **Run the notebooks in order:**

   **Step 1: Data Cleaning**
   - Open `SCRIPTS/1_cleaning.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will clean the raw dataset and output `DATA/final_data/cleaned_vaccine_data`

   **Step 2: Exploratory Analysis**
   - Open `SCRIPTS/2_exploratory_plots.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will generate descriptive statistics and visualizations in `README.md` in the DATA folder

   **Step 3: Machine Learning Models**
   - Open `SCRIPTS/3_model.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will perform the regression and statistical analysis used in our significance test and generate performance visualizations in `OUTPUT/model visualizations/`

**Note:** If using Google Colab, upload the dataset files `merged_influenza_presidents_data.csv` and `merged_vaccination_presidents_data` to the `/content/` directory before running the notebooks.



