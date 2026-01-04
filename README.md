# Sensory Data Analysis with Python

This repository contains Jupyter notebooks demonstrating various statistical and machine learning techniques for sensory data analysis. All these contents are part of the book chapter "Statistics and Multivariate Analysis" in the book "Sensory Evaluation of Foods: Methodologies, Data Analysis and Industrial Applications." 

The notebooks cover visualization, ANOVA, conjoint analysis, factor analysis, discriminant analysis, PCA, cluster analysis, PLS regression/DA, artificial neural networks, and fuzzy logic.

## Prerequisites

Before you begin, make sure you have the following:
- A computer running macOS, Linux, or Windows
- Internet connection for downloading packages

## Setup Instructions

Follow these detailed steps to set up your environment and run the notebooks:

### Step 1: Install Miniconda

Miniconda is a minimal installer for conda. It includes conda, Python, and a small number of useful packages.

**For macOS:**
1. Visit [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)
2. Download the macOS installer (choose the appropriate version for your Mac: Intel or Apple Silicon)
3. Open the downloaded `.pkg` file and follow the installation wizard
4. Restart your terminal after installation

**For Linux:**
1. Visit [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)
2. Download the Linux installer (choose the appropriate version for your system)
3. Open a terminal and navigate to the download directory
4. Run: `bash Miniconda3-latest-Linux-x86_64.sh` (replace with your downloaded filename)
5. Follow the installation prompts
6. Restart your terminal or run: `source ~/.bashrc`

**For Windows:**
1. Visit [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)
2. Download the Windows installer (`.exe` file)
3. Run the installer and follow the installation wizard
4. Make sure to check "Add Miniconda3 to my PATH environment variable" during installation (or add it manually later)

### Step 2: Open Terminal/Command Prompt

**For macOS/Linux:**
- Open the Terminal application (found in Applications > Utilities on macOS, or use your system's application launcher on Linux)

**For Windows:**
- Open **Anaconda Prompt** (not the regular Command Prompt)
  - You can find it by searching for "Anaconda Prompt" in the Start menu
  - Alternatively, if you added conda to PATH, you can use Command Prompt or PowerShell

### Step 3: Create a New Conda Environment

Create a new conda environment named `sensory` with Python 3.12:

```bash
conda create -n sensory python=3.12
```

This command will:
- Create a new isolated environment named `sensory`
- Install Python 3.12 in that environment
- Keep this environment separate from your system Python and other projects

You may be prompted to confirm the installation. Type `y` and press Enter to proceed.

### Step 4: Activate the Environment

After creating the environment, you need to activate it:

```bash
conda activate sensory
```

**Note:** 
- On macOS/Linux, your terminal prompt should now show `(sensory)` at the beginning
- On Windows (Anaconda Prompt), you should also see `(sensory)` in your prompt
- If you're using a regular Command Prompt on Windows and conda isn't recognized, use Anaconda Prompt instead

### Step 5: Install Required Packages

Navigate to the directory containing this README file and the `requirements.txt` file:

```bash
cd path/to/sensory_multivariate_analysis
```

Replace `path/to/sensory_multivariate_analysis` with the actual path to the `sensory_multivariate_analysis` folder on your computer.

Then, install all required packages using pip:

```bash
pip install -r requirements.txt
```

This will install all the necessary packages used across the notebooks:
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computing
- **matplotlib**: Basic plotting
- **seaborn**: Statistical visualizations
- **scipy**: Scientific computing and statistical functions
- **statsmodels**: Statistical modeling
- **scikit-learn**: Machine learning algorithms
- **patsy**: Design matrices for statistical models
- **openpyxl**: Reading Excel files (.xls, .xlsx)
- **factor-analyzer**: Factor analysis
- **tensorflow**: Deep learning (for neural networks)
- **scikit-fuzzy**: Fuzzy logic operations

**Note:** The installation may take several minutes, especially for TensorFlow which is a large package. Be patient and wait for the installation to complete.

### Step 6: Open Notebooks in Your Preferred IDE

You can use any IDE or editor that supports Jupyter notebooks. Here are some popular options:

**Option A: Jupyter Notebook (Web-based)**
- Launch Jupyter Notebook from the terminal:
  ```bash
  jupyter notebook
  ```
- This will start the Jupyter server and open it in your default web browser
- Navigate to the notebook files and click to open them

**Option B: JupyterLab (Enhanced web interface)**
- Launch JupyterLab from the terminal:
  ```bash
  jupyter lab
  ```
- Provides a more modern interface with file browser, terminal, and notebook support

**Option C: VS Code (Visual Studio Code)**
- Install the Python extension and Jupyter extension in VS Code
- Open the `sensory_multivariate_analysis` folder in VS Code
- Click on any `.ipynb` file to open and run it directly in VS Code
- Make sure to select the `sensory` conda environment as your Python interpreter (bottom-right corner of VS Code)

**Option D: PyCharm**
- Open the `sensory_multivariate_analysis` folder as a project in PyCharm
- Configure the Python interpreter to use the `sensory` conda environment:
  - Go to Settings/Preferences > Project > Python Interpreter
  - Select the `sensory` environment
- Open any `.ipynb` file - PyCharm has built-in Jupyter notebook support

**Option E: Cursor**
- Open the `sensory_multivariate_analysis` folder in Cursor
- Install the Jupyter extension if needed
- Open any `.ipynb` file to work with notebooks
- Select the `sensory` conda environment as your Python interpreter

**Option F: Other IDEs**
- Most modern IDEs (Spyder, Atom with Hydrogen, etc.) support Jupyter notebooks
- Make sure to configure your IDE to use the `sensory` conda environment as the Python interpreter
- Install any required Jupyter/notebook extensions for your IDE

**Important:** Regardless of which IDE you choose, make sure it's configured to use the `sensory` conda environment you created in Step 3. This ensures all the packages you installed are available.

### Step 7: Open and Run Notebooks

1. Open any notebook file (`.ipynb`) in your chosen IDE
2. The notebooks are numbered in order:
   - `0_visualization.ipynb`: Data visualization
   - `1_ANOVA_CochranQ.ipynb`: ANOVA and Cochran's Q test
   - `2_Conjoint_analysis.ipynb`: Conjoint analysis
   - `3_Factor_analysis.ipynb`: Factor analysis
   - `4_Discriminant_analysis.ipynb`: Linear discriminant analysis
   - `5_PrincipalComponentAnalysis.ipynb`: Principal component analysis
   - `6_Cluster_analysis.ipynb`: Cluster analysis
   - `7_PLSR_PLSDA.ipynb`: Partial least squares regression and discriminant analysis
   - `8_ArtificialNeuralNetwork.ipynb`: Neural networks
   - `9_Fuzzy_logic.ipynb`: Fuzzy logic analysis

3. To run cells in the notebook:
   - **Jupyter/JupyterLab**: Click on a cell and press `Shift + Enter` to run it, or use the toolbar buttons
   - **VS Code**: Click the "Run Cell" button above each cell, or press `Shift + Enter`
   - **PyCharm**: Use the play button next to each cell, or press `Shift + Enter`
   - **Cursor**: Similar to VS Code, use the run buttons or `Shift + Enter`
   - **Other IDEs**: Check your IDE's documentation for Jupyter notebook shortcuts
4. To run all cells, most IDEs have a "Run All" option in the cell menu or toolbar

## Important Notes

- **Data Files**: Make sure the `data/` folder is in the same directory as the notebooks. The notebooks expect data files to be in a `data/` subdirectory.
- **Environment Activation**: Every time you open a new terminal/command prompt to work with these notebooks, remember to activate the environment first: `conda activate sensory`
- **Package Updates**: If you encounter any issues, you can try updating packages: `pip install --upgrade -r requirements.txt`

## Troubleshooting

**Problem: `conda` command not found**
- **Solution**: Make sure Miniconda is properly installed and added to your PATH. On Windows, use Anaconda Prompt instead of regular Command Prompt.

**Problem: Packages fail to install**
- **Solution**: Try installing packages one by one to identify which package is causing issues. Some packages like TensorFlow may require specific versions.

**Problem: Notebooks don't open or run in your IDE**
- **Solution**: 
  - Make sure you've activated the `sensory` environment and installed all packages
  - For Jupyter/JupyterLab: Make sure you're in the correct directory and try: `python -m jupyter notebook` or `python -m jupyter lab`
  - For VS Code/PyCharm/Cursor: Make sure the IDE is configured to use the `sensory` conda environment as the Python interpreter
  - Check that the Jupyter extension/plugin is installed in your IDE

**Problem: Import errors when running notebooks**
- **Solution**: Make sure you've activated the `sensory` environment and installed all packages from `requirements.txt`. Verify installation with: `pip list`

## Getting Help

If you encounter any issues not covered here, please check:
1. That all steps were followed correctly
2. That your Python version is 3.12 (check with: `python --version`)
3. That all packages are installed (check with: `pip list`)

## License

This repository is for educational and research purposes.

