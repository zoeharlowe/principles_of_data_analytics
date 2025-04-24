# Principles of Data Analytics: Iris Dataset
by Zoe McNamara Harlowe.

This is my submission for the assessment of ATU module Principles of Data Analytics for the HDip in Computing in Data Analytics. 
This repository guides you through an investigation of the classic Iris dataset. 

---

## Table of Contents

1. [Prerequisites](#prerequisites)  
2. [Setup](#setup)
3. [Technologies](#technologies)
4. [Libraries](#libraries)
5. [Project Structure](#project-structure)    
6. [Tasks](#tasks)  

---

## Prerequisites

- Python 3.7 or higher  
- Required packages (listed in `requirements.txt`):  
  ```bash
  numpy
  matplotlib
  seaborn
  scikit-learn
  pandas
  scipy
---

## Setup

**View the repository online using Github Codespaces:**
1. Sign up for a free Github account.
2. Go to the repository page in your browser.
3. Click the green 'Code' button.
4. Click the 'Codespaces' tab.
5. Click 'Create New Codespace' on main.


**Or you can clone the repository onto your own machine:**
1. In Commander, clone the repo and change directory:
```bash 
git clone <https://github.com/zoeharlowe/principles_of_data_analytics>
cd <principles_of_data_analytics>
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Launch the Jupyter Notebook tasks.ipynb locally:
```bash
jupyter notebook tasks.ipynb
```

## Technologies

- Python
- Git
- Github
- Codespaces
- Jupyter

---

## Libraries

- Matplotlib (Pyplot): https://matplotlib.org/stable/tutorials/pyplot.html
- Numpy: https://numpy.org/doc/2.2/
- Scikitlearn: https://scikit-learn.org/stable/user_guide.html
- Pandas: https://pandas.pydata.org/docs/
- Seaborn: https://seaborn.pydata.org/
- Scipy: https://docs.scipy.org/doc/scipy/

--- 

## Project Structure
Principles of Data Analytics:
- .gitignore
- README.md            
- requirements.txt      
- tasks.ipynb:

    [Imports](tasks.ipynb#imports)

    [Task 1: Source the Data Set](tasks.ipynb#task-1-source-the-data-set)

    [Task 2: Explore the Data Structure](tasks.ipynb#task-2-explore-the-data-structure)

    [Task 3: Summarise the Data](tasks.ipynb#task-3-summarise-the-data)

    [Task 4: Visualise Features](tasks.ipynb#task-4-visualise-features)

    [Task 5: Investigate Relationships](tasks.ipynb#task-5-investigate-relationships)

    [Task 6: Analyse Relationship](tasks.ipynb#task-6-analyse-relationship)

    [Task 7: Analyse Class Distributions](tasks.ipynb#task-7-analyse-class-distributions)
    
    [Task 8: Compute Correlations](tasks.ipynb#task-8-compute-correlations)

    [Task 9: Fit a Simple Linear Regression](tasks.ipynb#task-9-fit-a-simple-linear-regression)

    [Task 10: Too Many Features](tasks.ipynb#task-10-too-many-features)

---

## Tasks

#### Task 1
- **File:** [Task 1: Source the Data Set](tasks.ipynb#task-1-source-the-data-set)
- **Description:** Import the Iris dataset and explain the structure returned by `load_iris()`.  
- **References:** [Raw version of Iris Dataset (from Github user Curran)](https://gist.githubusercontent.com/curran/a08a1080b88344b0c8a7/raw/0e7a9b0a5d22642a06d3d5b9bcbad9890c8ee534/iris.csv)

#### Task 2
- **File:** [Task 2: Explore the Data Structure](tasks.ipynb#task-2-explore-the-data-structure)  
- **Description:** Print and explain the dataset’s shape, first and last five rows, feature names, and target class labels.  
- **References:** [StackOverflow post to research `head()` and `iloc()` method](https://stackoverflow.com/questions/25254016/pandas-get-first-row-value-of-a-given-column)

    Microsoft Copilot to learn about the `np.unique()` function.

#### Task 3
- **File:** [Task 3: Summarise the Data](tasks.ipynb#task-3-summarise-the-data) 
- **Description:** Calculate mean, minimum, maximum, standard deviation, and median for each feature. 
- **References:** [Pandas `df.describe()` documentation](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.describe.html)

#### Task 4
- **File:** [Task 4: Visualise Features](tasks.ipynb#task-4-visualise-features) 
- **Description:** Plot histograms for each feature with appropriate titles and axis labels.  
- **References:** [Matplotlib documentation on `plt.hist()`](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.hist.html)

#### Task 5
- **File:** [Task 5: Investigate Relationships](tasks.ipynb#task-5-investigate-relationships)  
- **Description:** Create a colour‑coded scatter plot for two chosen features.  
- **References:** [Matplotlib documentation on `plt.scatter()](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html)

#### Task 6
- **File:** [Task 6: Analyse Relationship](tasks.ipynb#task-6-analyse-relationship)
- **Description:** Fit and overlay a regression line on the scatter plot using `numpy.polyfit`.  
- **References:** [Matplotlib documentation on `np.polyfit`](https://numpy.org/doc/stable/reference/generated/numpy.polyfit.html) 

    Ian McLoughlin Week 9 Video 2: Numpy's Polyfit

#### Task 7
- **File:** [Task 7: Analyse Class Distributions](tasks.ipynb#task-7-analyse-class-distributions)
- **Description:** Draw box‑plots of petal lengths for each of the three classes.  
- **References:** [ChatGPT to help with colour customisation of boxplots](https://chatgpt.com/share/680a218e-7ff0-8000-9562-e0c163ea71f7)

    [GeeksForGeeks article for producing multiple boxplots on one set of axes](https://www.geeksforgeeks.org/box-plot-in-python-using-matplotlib/)

#### Task 8
- **File:** [Task 8: Compute Correlations](tasks.ipynb#task-8-compute-correlations)
- **Description:** Compute feature correlation coefficients and display them as a heatmap.  
- **References:** [Documentation on `np.corrcoef()`](https://numpy.org/doc/stable/reference/generated/numpy.corrcoef.html)

    [Pandas documentation on the `df.corr()` method](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.corr.html)

    [Statology article explaining the correlation coefficient](https://www.statology.org/correlation-in-python/)

    [Matplotlib documentation on annotated heatmaps and the `plt.imshow()` method](https://matplotlib.org/stable/gallery/images_contours_and_fields/image_annotated_heatmap.html)

    [ChatGPT to research the LinearSegmentedColorMap module for the heatmap](https://chatgpt.com/share/67ffaf4d-5d08-8000-acf8-bd59f1760cbe)

#### Task 9
- **File:** [Task 9: Fit a Simple Linear Regression](tasks.ipynb#task-9-fit-a-simple-linear-regression)
- **Description:** Calculate the $R^2$ for your two chosen features, recreate the regression scatter plot, and annotate it with the $R^2$ value.
- **References:** [Wikipedia article explaining simple linear regression](https://en.wikipedia.org/wiki/Simple_linear_regression)

    [Scipy stats.linregress documentation](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.linregress.html)

    Ian McLoughlin Week 11 Video 3: R2 By hand

#### Task 10
- **File:** [Task 10: Too Many Features](tasks.ipynb#task-10-too-many-features)  
- **Description:** Create a pairplot using Seaborn to display each feature's relationship with each other using an appropriate title and axis labels.
- **References:** [Seaborn documentation on pairplots](https://seaborn.pydata.org/generated/seaborn.pairplot.html)

    [GeeksForGeeks article explaining pairplots](https://www.geeksforgeeks.org/python-seaborn-pairplot-method/)

    [YouTube video explaining the difference between KDEs and histograms when using pairplots](https://www.youtube.com/watch?v=cpZExlOKFH4)


*This README file was created with the help of ChatGPT: https://chatgpt.com/share/680a218e-7ff0-8000-9562-e0c163ea71f7*