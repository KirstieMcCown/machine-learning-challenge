# Machine Learning Challenge - Exoplanet Exploration
![Header](images/header.jpg)<br>

Welcome to my project repo! 
Feel free to take a look around the repo folders!<br>
This project is creating machine learning models capable of classifying candidate exoplanets from a raw dataset. 

If you are interested, you can find out more information about the data here:<br>
* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)<br><br>
* [Data Dictionary](https://exoplanetarchive.ipac.caltech.edu/docs/API_kepcandidate_columns.html)<br><br>

## The Models
<hr>
When viewing the data and data dictionary, it was clear that there was some values within the dataset that would not be relevant or applicable for the model we wanted to create, and there were also some values that looked to potentially have more importance when creating a model to classify candidate exoplanets. Therefore two types of models were used to compare results, and along with this, each model was adjusted to allow a slightly different selection of data to be analysed to see if we could achieve better results by narrowing down the scope of the model(s)
<hr>
<br>

<h3>Logistic Regression</h3>
<p>Two logistic regression models were created within notebook files, the notebook files are called 'logistic_model.ipynb', and 'logistic_model_compare.ipynb'. The models have also been saved as '.sav' files. <br>
In 'logistic_model.ipynb', features have been selected specifically to evaluate, based off information within the data dictionary. 
<br><br>
Within 'logistic_model_compare.ipynb', we have used all columns (other than the selected column for our y value), to evaluate. <p>
<br><br>
<hr>
<h3>Support Vector Machine</h3>
<p>Two support vector machines were created within notebook files, the notebook files are called 'svm_model.ipynb', and 'svm_model_compare.ipynb' The models have also been saved as '.sav' files. <br>
In 'svm_model.ipynb', features have been selected specifically to evaluate, based off information within the data dictionary. 
<br><br>
Within 'svm_model_compare.ipynb', we have used all columns (other than the selected column for our y value), to evaluate.<p>



<br><br>
<hr>
<h2>Analysis</h2>

Initially it appears as though selecting specific features to evaluate does not have a better predictive score than using all records within the data as both our testing and training data score is around the 0.75 mark, and once tuning the model(s) parameters using "GridSearchCV", this stays the same; whilst utilising all of our data gives us an overall score approximately 10% higher with both our testing and training scores approximately 0.85.
<br>
Therefore, when creating a machine learing model for this data set, utilising all values within the dataset gives us a better result, and better ability to classify candidate exoplanets - these results are across both the Logistic Regression and Support Vector Machines, and the indication that scores are the same utilising both methods, tells us that these machines can be trusted, to be accurate in classifying candidate exoplanets.




<br><br><br>








### Created With<hr>
This project was created using the following:<br>
* Python
* Scikit-Learn
* Pandas
* joblib




