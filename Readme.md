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


----

### Kind of plots presents in this repo - notebooks with codes used to develop this plots


**ydata-profiling**

[1 link-data-profiling](https://github.com/joseortegalabra/exploratory-data-analysis/tree/main/1_ydata_profiling)


**Univariate Analysis**

[1 descriptive statistics table](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/2_plots_univariate_analysis/1_table_statistics.ipynb)

[2 histograms](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/2_plots_univariate_analysis/2_histogram.ipynb)

[3 kernel density + histograms](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/2_plots_univariate_analysis/3_kernel_density.ipynb)

[4 original data trend](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/2_plots_univariate_analysis/4_tendency.ipynb)

[5 boxplots with monthly aggregation](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/2_plots_univariate_analysis/5_boxplot_months.ipynb)

[6 original vs smoothed data trend](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/2_plots_univariate_analysis/6_smooth_data.ipynb)

[7 Autocorrelation and partial autocorrelation functions-v1](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/2_plots_univariate_analysis/7_autocorrelations.ipynb)

[7 Autocorrelation and partial autocorrelation functions-v2](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/2_plots_univariate_analysis/7_autocorrelations_v2.ipynb)

[8 Other analyzes for time series-v1](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/2_plots_univariate_analysis/8_partial_autocorrelacions.ipynb)

[8 Other analyzes for time series-v2](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/2_plots_univariate_analysis/8_partial_autocorrelations-v2.ipynb)


**Bivariate Analysis**

[1 correlations](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/3_plots_bivariate_analysis/1_correlations_pearson.ipynb)

[2 scatter plots](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/3_plots_bivariate_analysis/2_scatter_dispersion.ipynb)

[3 correlations features with lag](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/3_plots_bivariate_analysis/3_correlations_features_lag_target.ipynb)

[4 Multivariate parallel plot](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/3_plots_bivariate_analysis/4_parallel.ipynb)


**Segmentation Analysis**

[0 generate data segmentation](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/4_plots_segmentation_analysis/0_intro_get_data.ipynb)

[1 segmented data distribution](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/4_plots_segmentation_analysis/1_distribution_segmentation.ipynb)

[2 descriptive statistical table segmented data](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/4_plots_segmentation_analysis/2_table_statistics_segmentation.ipynb)

[3 histograms and boxplots segmented data](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/4_plots_segmentation_analysis/3_histogram_boxplots_segmentation.ipynb)

[4 trend segmented data](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/4_plots_segmentation_analysis/4_tendency_segmentation.ipynb)

[5 segmented data correlations](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/4_plots_segmentation_analysis/5_correlations_segmentation.ipynb)

[6 scatter plots segmented data](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/4_plots_segmentation_analysis/6_scatter_segmentation.ipynb)

[7 parallel plot only when target is segmented](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/4_plots_segmentation_analysis/7_parallel_target_segmentation.ipynb)


**Categorical Analysis**

[0 generate categorical data](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/5_plots_categorical_analysis/0_intro_get_data.ipynb)

[2 crosstab frequency features and target](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/5_plots_categorical_analysis/2_crosstab_freq_features_target.ipynb)

[3 frequency between 2 categorical features](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/5_plots_categorical_analysis/3_freq_x_cat_x_cat.ipynb)

[4 univariate analysis categorical features vs continuous target](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/5_plots_categorical_analysis/4_univariate_analysis_x_cat_y_cont.ipynb)

[5 univariate analysis categorical features vs categorical target](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/5_plots_categorical_analysis/5_univariate_analysis_x_cat_y_cat.ipynb)

[6 bivariate analysis categorical features vs continuous target](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/5_plots_categorical_analysis/6_bivariate_analysis_x_cat_y_cont.ipynb)

[7 bivariate analysis categorical features vs categorical target](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/5_plots_categorical_analysis/7_bivariate_analysis_x_cat_y_cat.ipynb)

[8 parallel plot features categorical vs categorical target](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/5_plots_categorical_analysis/8_parallel_x_cat_y_cat.ipynb)

[9 woe iv - categorical features vs binary target](https://github.com/joseortegalabra/exploratory-data-analysis/blob/main/5_plots_categorical_analysis/9_woe_iv_x_cat_y_cat.ipynb)
