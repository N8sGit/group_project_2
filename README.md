## Project Overview
# This project explored using Machine Learning to predict the quality of Vinho Verde wine (Red and White) from Portugal's northwest region. 

### Team members
* Elizabeth Arias <br/>
* Dawn Kim <br/>
* Christian Leon <br/>
* Nathan Anecone <br/>
* Ian Cody <br/>
* Kyle Prudente <br/>

This project utilizes two datasets from the kaggle.com in CSV format named "wine_data_white.csv" and "wine_data_red.csv" that were combined into "wine_data_both.csv".

The program requests an upload of "wine_data_both.csv".
A data frame called "combined_data" isolates only the necessary columns and drops the 'NaN' values.
Variables kept for the analysis of this project are as follows:

- 'Index',  <br/>
- 'fixed acidity',  <br/>
- 'volatile acidity', <br/> 
- 'citric acid', <br/>
- 'residual sugar',  <br/>
- 'chlorides',  <br/>
- 'free sulfur dioxide', <br/>
- total sulfur dioxide', <br/> 
- 'density',  <br/>
- 'pH',  <br/>
- 'sulphates',  <br/>
- 'alcohol', <br/>
- 'quality' <br/>
       
Exploratory data analysis involved the following methods:
* Describe <br/>
* Correlation heatmap <br/>
* box plot <br/>
* histogram charts <br/>
* p-value analysis <br/>
* violinplots <br/>


The following steps were taken:
1. The target variable of 'Quality' was analyzed for correlation and highly correlated variables were removed '(Free sulfur dioxide' and 'density'.
2. The distribution of all the variables were reviewed and outliers were removed for the purposes of training the model
3.  


A function is created to graph the .....
Random Forest models are created for ..... showing the predicted values for the next .. years.

Dataset

### Tools for Analysis
- Jupyter Notebook
- Google Collab
- Github
- Kaggle


Started with project ideation, sourcing data & transforming it using excel and python to a usable dataframe and csv file. Then used Power BI to quickly gather insights on the downloaded dataset and assess the feasibility of our hypothesis. Python was used for formatting and exploratory data analysis. The new layout was stored as a standard CSV file that was read into our code as a dataframe. Github was used for code repository, presentation deck and README file. Finally built visualizations using Matplotlib. Both top-down and bottom-up approachs were adopted to define the narrative, synthesizing of information/charts, and ensuring they answer the questions we set out to address.

The conclusions were...



References

Kaggle.com
P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis. Modeling wine preferences by data mining from physicochemical properties. In Decision Support Systems, Elsevier, 47(4):547-553, 2009.
