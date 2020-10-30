# Machine Learning Challenge - Exoplanet Exploration
![Header](Images/Header.PNG)<br>

Welcome to my project repo! 
Feel free to take a look around the repo folders! 
This is creating machine learning models capable of classifying candidate exoplanets from a raw dataset. 

If you are interested, you can find out more information about the data here:<br>
* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)<br><br>
* [Data Dictionary](https://exoplanetarchive.ipac.caltech.edu/docs/API_kepcandidate_columns.html)<br><br>

## The Models
<hr>
When viewing the data and data dictionary, it was clear that there was some values within the dataset that would not be relevant or applicable for the model we wanted to create, and there were also some values that looked to potentially have more importance when creating a model to classify candidate exoplanets. Therefore two types of models were used to compare results, and along with this, each model was adjusted to allow a slightly different selection of data to be analysed to see if we could achieve better results by narrowing down the scope of the model(s)
<hr>
<br>

<h3>Logistic Regression</h3>
<h5>Two logistic regression models were created, called 'logistic_model.ipynb', and 'logistic_model_compare.ipynb' <br>
In the 'logistic_model.ipynb', features have been selected specifically to evaluate, based off information within the data dictionary. 
<br><br>
Within 'logistic_model_compare.ipynb', we have used all columns (other than the selected column for our y value), to evaluate. 
<br><br>
Initially it appears as though selecting specific features to evaluate (logistic_model.ipynb) does not have a better predictive score than using all records within the data as both our testing and training data score is around the 0.75 mark, and once tuning the models parameters using "GridSerchCV", this stays the same; whilst using all columns of data (logistic_model_compare.ipynb) gives us an overall score approximately 10% higher with both our testing and training scores approximately 0.85
<br>
Therefore, when using a logistic regression model for this data set, utilising all values within the dataset gives us a better result, and better ability to classify candidate exoplanets.




<br><br><br>
<hr>
<h3>Support Vector Machine</h3>





<br><br><br>





### Created With<hr>
This project was created using the following:<br>
* Python
* Scikit-Learn
* Pandas
* joblib




