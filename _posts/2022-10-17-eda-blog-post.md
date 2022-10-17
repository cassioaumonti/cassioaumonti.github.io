
## Third Blog Post - EDA version

This blog post goes over Exploratory Data Analysis (EDA).

I will try to answer the following questions: write up the strategy you use for EDA. What is your overall goal when doing an EDA? What methods do you think are important? What things do you try to look for?

The concept of EDA is connected to the idea of looking at data without making any assumptions, as a prior analysis. It is helpful to find errors in the observations and identify evident patterns and relationships among variables. Therefore, it is clear that EDA is an important part of a Data Scientist actions, since working with unknown data is quite frequent and EDA may also be used to validate results according to the business goals. Hence, it is a fundamental step for any Data Scientist.  
  
  Some methods can be applied when doing basic EDA, graphical and non-graphical approaches, usually done via programming language as R, SAS, or Python, such as: 

  - Univariate, in which there is just one variable, continuous, discrete, or categorical. **The numerical analysis** for a single variable consists in summarizing the main statistics of center and spread (for continuous and discrete), for example, mean and median (for center) and variance and interquartile range (for spread). For categorical variable, the contingency table counting the frequency of the categories is the main metric. The **graphical analysis** for a single variable consists in plotting it using a histogram and boxlpot. The former is a bar plot that count the frequency of observations considering classes of data (for discrete and continuous) or categories (for categorical data). A boxplot summarizes graphically the 5-numbers summary (minimum, first quartile, median, third quartile, and maximum).
  
  - and Multivariate, also can be numerical and graphical, which is applied to more than one single variable. Usually, multivariate **numerical analysis** is done showing the relationship between two or more variables via two-way contingency table (for categorical data) or some statistics such as correlation coefficient, generally, the most utilized correlation coefficient is Pearson's correlation. It measures the linear correlation between variables in the data set and presents values between -1 and 1, which correlations close to -1 (or negative) indicates that as one variable increases its value implies in the reduction on the values of the other variable. Additionally for numerical analysis, some more advanced techniques can be used in the multivariate scheme such as clustering algorithms, for instance, the use of k-means, unsupervised learning algorithm where observations are assigned into k groups, is widely spread, as well as linear regression for EDA and inference purposes. Even the predictions of such models can be used to analyze if the data can contain unusual information. For **graphical analysis**, scatter plots and line plots are the most used to identify relationship between variables. Comparing similarities among variables through their distributions and density plots is also common, using histograms and density graphs.

To perform EDA, the Data Scientist can follow some basic steps and principles:    
    
  -1. Before any basic analysis, we should understand the business question and try to speak to people to obtain context about the data that helps inform the goals and where to focus. For instance, the Data Scientist should look for answers to these questions: is it about a prediction or classification task? Should inference be considered? What are the key variables?    

  -2. Once questions have been answered, the Data Scientist may look for **missing data**, that should be the very first step of a basic EDA. Missing data is so important that there is a field in statistics designed specifically to study missing data and ways to replace them, it is called *Imputation*. Usually, the best approach for this step is try to understand why the data is missing. However, this phase of the EDA is not always simple.    
   
  -3. Description of Sample and Variables is the second step of EDA, meaning to separate the variables into the listed data types above, among continuous, discrete, or categorical data. This steps assists in deciding which graphic types and numerical metrics we can use to perform the EDA.    
   
  -4. Identify the **Shape of the Data** is the next step. The shape of the data, based on the collected sample, is obtained using histogram or density plots. These graphical tools, including the boxplot, help identify the distribution of the data set, either the probability density function (PDF) for continuous data or probability mass function (PMF) for discrete data. They are also important to check if there is seasonality to the variable or a trend over time. The main metrics associated to distributions are skewness, the assimetry associated to the extremes of the distribution, and if there is any pattern in the PDF such as a gap or more than one peak (multimodal).    
   
  -5. Check out for **Significant Correlations**. As mentioned above, correlation coefficient measure the relationship among variables in a multivariate scheme. Pearson's correlated coefficient is the most used method for measuring linear relationship and it is represented by the Greek letter $\rho$. If the data set is a time series data, for instance, the metrics is called autocorrelation, referring to the residuals not being considered independent. Many tests using the Shape of the data, or the distribution of the data, help identify such property. Autocorrelation shows the relationship between a current signal value and its previous values.     
   
  -6. **Identify Outliers**: Outliers are unusual information present in the data set and they are considered significantly different form the main chunk of the data. They can be detected via boxplot, the observations below the minimum data point or above the maximum data point. In the EDA, it is fundamental to detect and treat outliers accordingly due to their high potential of interfering on the subsequent tasks following the EDA. Outliers may occur naturally, however, and they can be rightful representatives of the data distribution. Hence, they should be understood and treated with caution.


Hopefully, this blog post can serve you with your EDAs.


Thank you for reaching this far, see you next time!









