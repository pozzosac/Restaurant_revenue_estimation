### DSI-13 Hackathon, Restaurant Revenue Prediction, Sid Carter
### Predict annual restaurant sales based on objective measurements

The instant DSI-13 exercise is based on a Kaggle competition with an objective to find a mathematical model to increase the effectiveness of investments in new restaurant sites. In particular build a model that uses  demographic, real estate, and commercial data,to predict the annual  sales for thousands of prospective restaurant businesses at regional sitesaround the world.

The data was provided by Kaggle.

### The project

The project's key workstreams:
<ol>
<li>Download the data.</li>
<li>Prepare and stage the data for use in regressor predictive models.</li>
<li>Build at least two models that use predictor data from the Kaggle database in order to produce predictions of annual sales for   prospecitve restaurants.</li>
   

### EDA activities

EDA activities were limited because the presented data 'train' data possessed high integrity and was sound.  The 'train' data comprised 137 observations with 43 indpendent variables and a dependent variable, revenue.  The brunt of the data was described as "three categories of obfuscated data: Demographic data, Real estate data, and Commercial data."  The lack of data dictionary information limited directed feature engineering.  A couple variables (City-type and Restaurant-type) were dummified.
    

The jupyter notebook presents several EDA tables and charts that were relied upon to inspect and validate the structure of the data - histograms, scatterplots, correlation tables, etc.


### Modeling activities and conclusions

Three models were produced and evaluated for predictive accuracy:

<ol>
<li>Multi-linear</li>
<li>K Nearest Neighbors</li>
<li>Random Forest</li>
</ol>

A grid-search algorithm was used for the KNN and Random Forest models.  The Random Forest model was most effective of the three models considered, as illustrated by the rmse for the three models presented below:

<ol>
<li>rmse_linear_regression_test:  1,773,509</li>
<li>rmse_knn_test:                             379,674</li>
<li>rmse_random_forest-test:        182,315</li>
<ol>
