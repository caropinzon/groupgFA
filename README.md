# groupgFA
Group G Financial Analytics MBD 2016

###Welcome
Welcome to Group G's Financial Analytics Innovation and beyond in Big Data System for Model Development System.

We have built 5 distinct algorithms to harness and wrangle two different datasets (dev.csv or MBD_FA2.csv). There is a selection of both human-assisted step-by-step guides to give you control when running the algorithms, and other purely automatic algorithms.

###Installation
To install our package, just paste the folloing line in your terminal: **sudo pip3 install groupgfa**

###Implementation
For each of the different **algorithms** you only have to call them with a dataframe as the input. For example, you can perform the Automated Data Cleaning algorithm by typing groupgFA.autoClean(df) with a dataframe that you select.

These are the different algorithms you can implement along with their method names and some information about what they do.

A.1) Automated Data Cleaning **autoClean(df)**
  - NaN & Missing Values:
    - Replace NaN with mean of column.
    - Calculate the mean for each column
    - Determine which are the NaN values 
    - Replace NaN with mean of column
  - Outliers & Out of range: 
    - A data point significantly different from others in the same set. 
    - Remove outliers based on function.
    - Mean & SD to the median, scale distances by the median giving  us a better relative scale than from the mean.	  
  - Unreliable values, 
    - Non integer values are treated as errors, thus they are replaced with a NaN, and later with the mean of column. 
  - Exports csv file with clean variables

A.4.1) Automated Dummy Creation and Transformation with Automated Supervised Binning **autoVariableCreate(df)**
  - Creates Variables from all possible ratios, sums, multiplications, and differences between two variables from a subset of variables with a range of atleast 5. 
  - Binning and Dummy Variable Creation
  - Exports csv file with new variables


A.6) Automated method comparison and choosing **autoselectModel(df)**
  - Preparing Data for Model Selection Algorithm
  - Scaling Variables in Model
  - Cross Validation & Accuracy Measure Creation
    - Running 6 Different Models (sklearn)
      - AdaBoost
      - SVM
      - Gradient Boosting
      - Random Classifier
      - K-n-neighbors
      - SDG Classifier
  - Selecting Best Model Based on Accuracy

H.1) Human assisted Data Cleaning **humanClean(df)**
  - Replacement of NaN & Missing Values:
  - Normalization 
  - Exports csv file with clean variables

H.4) Human assisted variables and ratios creation **humanVariableCreate(df)**
  - Seperation of Target
  - Selection of equation to be applied
    - SUM
    - RATIO
    - PRODUCT
    - SUBTRACTION
    - MODULUS
  - Exports csv file with new variables
