# VaxxVote
##Contents of the Repository##
###Section 1: Software and Platform Section###
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

Make an H2 (##) section explaining the contents of the repository ● Section 1: Software and platform section ○ The type(s) of software you used for the project. ○ The names of any add-on packages that need to be installed with the software. ○ The platform (e.g., Windows, Mac, or Linux) you used. ● Section 2: A Map of your documentation. In this section, you should provide an outline or tree illustrating the hierarchy of folders and subfolders contained in your Project Folder, and listing the files stored in each folder or subfolder. ● Section 3: Instructions for reproducing your results. In this section, you should give explicit step-by-step instructions to reproduce the Results of your study. These instructions should be written in straightforward plain English, but they must be concise, but detailed and precise enough, to make it possible for an interested user to reproduce your results without much difficulty. N.B. This section will be crucial for the CS1 assignment, where you'll be required to reproduce the results of other groups. Therefore, make sure to explain this section thoroughly.

## Instructions for Reproducing the Results

1. **Clone the repository:**
   ```bash
   git clone https://github.com/srujanay18/SentiCook.git
   cd SentiCook
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
   - This will generate descriptive statistics and visualizations in `OUTPUT/exploratory/`

   **Step 3: Machine Learning Models**
   - Open `SCRIPTS/3_model.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will perform the regression and statistical analysis used in our significance test and generate performance visualizations in `OUTPUT/model visualizations/`

**Note:** If using Google Colab, upload the dataset file `Recipe Reviews and User Feedback Dataset.csv` to the `/content/` directory before running the notebooks.

