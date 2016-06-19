# groupgFA
Group G Financial Analytics MBD 2016

##Welcome
Welcome to Group G's Financial Analytics Innovation and beyond in Big Data System for Model Development System.

We have built 5 distinct algorithms to harness and wrangle two different datasets (dev.csv or MBD_FA2.csv). There is a selection of both human-assisted step-by-step guides to give you control when running the algorithms, and other purely automatic algorithms.

###Installation
To install our package, just paste the folloing line in your terminal: *sudo pip3 install groupgfa*

###Implementation
For each of the different *algorithms* you only have to call them with a dataframe as the input. For example, you can perform the Automated Data Cleaning algorithm by typing groupgFA.autoClean(df) with a dataframe that you select.

These are the different algorithms you can implement along with their method names.

A.1) Automated Data Cleaning *autoClean(df)*

A.4.1) Automated Dummy Creation and Transformation with Automated Supervised Binning *autoVariableCreate(df)*

A.6) Automated method comparison and choosing *autoselectModel(df)*

H.1) Human assisted Data Cleaning *humanClean(df)*

H.4) Human assisted variables and ratios creation *humanVariableCreate(df)*
