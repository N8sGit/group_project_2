## Project 2 Overview
# This project explored using Machine Learning to predict the quality of Vinho Verde wine (Red and White) from Portugal's northwest region. 

Started with project ideation, sourcing data & transforming it using excel and python to a usable dataframe and csv file. Then used Power BI to quickly gather insights on the downloaded dataset and assess the feasibility of our hypothesis. Python was used for formatting and exploratory data analysis. The new layout was stored as a standard CSV file that was read into our code as a dataframe. Github was used for code repository, presentation deck and README file. Finally built visualizations using Matplotlib. Both top-down and bottom-up approachs were adopted to define the narrative, synthesizing of information/charts, and ensuring they answer the questions we set out to address.

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
![image](https://github.com/N8sGit/group_project_2/assets/163077507/f2288b2f-539f-4987-970c-2575012f9110)
* Correlation heatmap <br/>
![image](https://github.com/N8sGit/group_project_2/assets/163077507/7823057f-4225-4b86-90cd-2bc1c8500369)
* box plot <br/>
![image](https://github.com/N8sGit/group_project_2/assets/163077507/0d480594-9f1c-46bc-a09f-9681cd6c3f01)
* histogram charts <br/>
![image](https://github.com/N8sGit/group_project_2/assets/163077507/95c84092-fd42-4ac6-8f86-b41885176f7c)
* violinplots <br/>
![image](https://github.com/N8sGit/group_project_2/assets/163077507/04ad41dc-3e4a-4821-8a9b-c05631f6545a)
* p-value analysis that did not provide any significant results <br/> 


The following steps were taken:
1. The target variable of 'Quality' was analyzed for correlation and highly correlated variables were removed '(Free sulfur dioxide' and 'density'.
2. The distribution of all the variables were reviewed and outliers were removed for the purposes of training the model
3.  

### Conclusion
The Key Takeaways are that alcohol is the best predictor for High quality wine using a Random Forest Model.

Dataset

### Tools for Analysis
- Jupyter Notebook
- Google Collab
- Github
- Kaggle


References

Kaggle.com
P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis. Modeling wine preferences by data mining from physicochemical properties. In Decision Support Systems, Elsevier, 47(4):547-553, 2009.
