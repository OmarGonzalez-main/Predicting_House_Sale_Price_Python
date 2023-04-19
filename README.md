<h3><br><br><br>Introduction</h3>
<p>
  This report presents the findings and outcomes of my data analysis project focused on predicting house sale prices in King County, USA. The dataset includes information on house sales between May 2014 and May 2015, with features such as the number of bedrooms, bathrooms, square footage, and more. The project aimed to develop a predictive model using various data analysis and machine learning techniques.
</p>

							
<h3>Data Wrangling</h3>
<p>
The data wrangling process involved the following steps:	
<ul>
<li>Importing necessary libraries and loading the dataset.</li>
<li>Identifying and handling missing values.</li>
<li>Checking for duplicates and removing them.</li>
<li>Converting data types when necessary.</li>
</ul>
</p>



<h3>Data Exploration</h3>
<p>
During the data exploration phase, the following steps were performed:
<ul>
<li>Descriptive statistics were calculated to gain insights into the data.</li>
<li>Visualizations were created to explore relationships between variables, such as:</li>
<li>Box plots to identify outliers.</li>
<li>Regression plots / Scatter Plots to examine the correlation between variables.</li>
<li>Correlation analysis was conducted to identify highly correlated features.</li>
</ul>
</p>



<h3>Hypothesis Testing</h3>
<p>
A t-test was performed to investigate the hypothesis that houses with more bedrooms have higher sale prices. The null hypothesis stated that there was no significant difference in the mean price between houses with different numbers of bedrooms. The alternative hypothesis claimed that there was a significant difference. The test resulted in a p-value significantly less than 0.05, leading to the rejection of the null hypothesis and the acceptance of the alternative hypothesis. We can therefore conclude that there is a relationship between the number of bedrooms and the sale price. We also examine this further in the project and see that price increases as the number of bedrooms reaches 8 before dropping with homes having more than 8 bedrooms.
</p>




<h3><br>Model Development and Refinement</h3>
<p>
Several models were developed and compared, including:<br>
<ul>
<li>Simple linear regression with one independent variable (square footage of living space).</li>
<li>Multiple linear regression with multiple independent variables.</li>
<li>Polynomial regression models of varying degrees.</li>
<li>Polynomial regression model with ridge regression.</li>
</ul>
A grid search was performed to optimize the hyperparameters for the polynomial model with ridge regression. The best performing model was the polynomial model of degree 2 with ridge regression with alpha = 0.001, which had an R-squared value of 0.7601.<br>
We could say then that the polynomial model with ridge regression was the best model but after some more evaluation using cross-validation, we see that the model that performs best is the polynomial model with an average r-squared of 0.7331 compared to 0.7193 to that of the polynomial model with ridge regression.
</p>



<h3><br>Conclusion and Key Findings</h3>
<p>The project successfully analyzed the King County House Sales dataset and developed a predictive model for house sale prices. The data wrangling, exploration, hypothesis testing, and model development steps provided valuable insights into the factors influencing house prices and the performance of various regression models. The selected polynomial model can be used as a basis for further refinement and improvement. Future work could involve exploring additional features, applying feature selection techniques, or experimenting with alternative modeling methods to further improve the model's performance.</p>
<p>Some key findings from this project :
<ul>
  <li>The average sale price of houses in King County was roughly $540,000</li>
  <li>The number of bedrooms does have a significant correlation with the sale price of homes. Price increases as the number of bedrooms increase to 8 but then decreases at 8 bedrooms and above.</li>
  <li>There does not seem to be a relationship between the number of times a house has been viewed and the sale price. Realistically we would expect the more expensive houses to be viewed less but this was not shown to be the case from our analysis.</li>
</ul>
</p>
