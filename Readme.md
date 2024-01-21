# EDA - Exploratory Data Analysis

## Goal
The idea is have a repository with codes templates to do a EDA that can be repeated for almost all diffents types of datasets


## Contents:
- Folder this differents types of exploratory analysis
- Notebooks with codes with differents analysis. 
- Important: The notebooks and notebooks are numerated to indicate the orden in which were writted but it not represent the order that it can be used to analyse the data
- Imporant 2: The notebooks try to be structed such as:
	- eda numbers: For example generate a dataframe with the correlations
	- eda plot-graph: generate a plot with plotly using as input the eda numbers or the data
	- eda graph - plotly: generate a plot with plotly using as input the eda numbers (when it is possible)
	- synthesize: join the previous code in a function that is parameterized and can be used with any dataset
    - So, to see the final codes develeop in the notebooks that can be used in any case, search all the function defined: Ex def function1(x, y, z)
- There is a folder output_eda where are saved the plots output of the eda. This output are not pushed but can be obtained running the codes


## Next steps automatization(the idea is it will be in other repo):
1. Create a script.py that will have all the codes develop in this repo
2. Use this codes and automatize the analysis. Create an app kind plug and play where return all the analysis done in a pdf or html file (for example using plotly) (Actually there is a script develop and a config file, and running this code can generate automatically the plots for EDA)
3.(optional) develop a web app that can pass a dataframe and define the parameters and do the analysis. It is possible with streamlit but it takes time (so far, not done)
4. Apply this analysis to a differents uses cases
5. The codes with the automatization are located in: https://github.com/joseortegalabra/automatic-exploratory-data-analysis


## Templates codes:
- There are a lot of functions that recibe a pandas dataframe and other parameters that each function needs and return a plotly figure
- Then with the plotly figure you can see in a jupyter notebok with the method fig.show() or you can saved it in a folder with the methods
fig.write_html to get a html interactive figure or fig.write_image to get a static image similar to other packages as matplotlib or seaborn
- In the script main.py the order is read the config file, then read the parameters since de config.json that you will use and finally call the function
to generate the plots to get a plotly figure and finally decide what to do (show, save html, save png, save pdf, etc)