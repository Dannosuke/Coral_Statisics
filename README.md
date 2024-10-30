Coral Statistics Toolkit
Welcome to the Coral Statistics Toolkit, a collection of Python tools designed to assist in analyzing coral cover data from .cpc files. This toolkit provides a range of functionalities, including statistical analysis of coral cover, diversity indices, and random file selection, all in an easy-to-use, GUI-based format.

Table of Contents
Overview
Features
Installation
Usage
Random File Selector
Coral Cover Analysis
Coral Cover Comparison
Requirements
License
Overview
This repository contains three primary scripts:

Random File Selector: A tool for selecting a random subset of files from a specified directory.
Coral Cover Analysis: Analyzes coral cover across multiple sites, transects, and depths, with exportable summaries in CSV format.
Coral Cover Comparison: Compares predicted coral cover annotations against actual data using statistical metrics and diversity indices.
Features
Graphical User Interface (GUI): Each script includes a Tkinter-based GUI for user-friendly interaction.
Data Sampling: Randomly select files from a directory by a specified percentage.
Coral Cover Analysis: Calculates site, transect, and depth-level coral cover summaries and exports data in CSV format.
Statistical Comparison: Evaluates predicted vs. actual coral cover using accuracy metrics and ecological diversity indices.
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/Dannosuke/Coral_Statistics.git
cd Coral_Statistics
Install the required Python libraries:

bash
Copy code
pip install numpy pandas scikit-learn scipy
Run any of the three scripts with Python:

bash
Copy code
python script_name.py
Usage
1. Random File Selector
This script allows users to select a random subset of files from a source directory and copy them to a target directory, with the option to specify the percentage of files.

Launch the script: random_file_selector.py
GUI Workflow:
Select the source and target folders.
Choose the percentage of files to copy.
Click "Copy Files" to execute the operation.
2. Coral Cover Analysis
This script calculates coral cover averages at site, transect, and depth levels within a selected folder structure. Data is organized into summaries and can be saved as CSV files.

Launch the script: coral_cover_analysis.py
GUI Workflow:
Select the main folder containing .cpc files.
Review calculated summaries in the GUI text box.
Save results as CSV files for site, transect, depth per site, and island-wide depth summaries.
3. Coral Cover Comparison
This tool compares actual vs. predicted coral cover data using metrics like accuracy, F1-score, Cohen's kappa, and Matthews correlation coefficient. It also calculates ecological diversity indices such as Shannon-Wiener, Simpson’s, and Chao1.

Launch the script: coral_cover_comparison.py
GUI Workflow:
Select folders for actual and predicted data.
Run the comparison, which displays metric results in the GUI text box.
Requirements
Python 3.x
Libraries: numpy, pandas, scikit-learn, scipy, tkinter
Install dependencies with:

bash
Copy code
pip install numpy pandas scikit-learn scipy
