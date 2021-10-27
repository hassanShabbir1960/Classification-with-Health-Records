# Classification-with-Health-Records


Dataset Description
This dataset includes information about over 100,000 medical appointments of different patients from different neighborhoods in Brazil, and this dataset discuss very important point that why a person makes a doctor appointment, receives all the instructions and no-show. 


<h3>Part I: Data prep:</h3>


<ul> This includes: </ul>

<li>Reading in data csv file </li>

<li>Cleanup data column names </li>

<li>Removed records with erroneous entries (e.g., negative ages, look at what people have done in Kaggle) </li>

<li>Created a test set of 20k records that you won’t touch again for the reminder of this project until Part III. Use stratified sampling on the No-show variable to ensure test set and training set class proportions are the same. Save the train and test sets as csv files in the processed_data directory. </li>

<li>Plotted the No-show variable against the other variables in the dataset as part of Exploratory Data Analysis </li>

<li>Created a preprocessing pipeline using scikit to prepare the data for the ML algorithms we will use. At a minimum, standardize numerical variables, transform categorical variables into one or more numerical values. You may apply other transformations that you think would be useful (e.g., logarithmic transformations).</li>




<h3>Part II: Classification Methods </h3>
<ul>  Here are the steps involved in this part </ul>  

<li> Using sklearn fit a DecisionTree, a RandomForest, a linear SVM and an SVM with a radial basis kernel to the transformed data. For now, use default parameters for each method. </li>

<li> Use 10 fold cross validation to estimate performance of each of the above methods using both accuracy and AUC as metrics. </li>

<li> Based on the above choose two of the ML methods and fit a model using 5 fold cross validation for model selection and 10 fold cross validation for model assessment. </li>

<li> Implemented gradient descent for a linear svm and test it on the training set. </li>



<h3>Part III: Ensembles </h3>
<ul>  Here are the steps involved in this part </ul>  

<li>Trained an AdaBoost classifier and compare its performance to the results obtained in Part II using 10 fold cross validation as before </li>

<li>Trained an xgBoost classifier and compare its performance to the results obtained in Part II </li>

<li>Chose a set of 5 or so classifiers, e.g., Decision Trees of diverse depths, linear SVMs over diverse subsets of features, RBF kernels with diverse bandwidths, Random Forests with diverse number of trees in their ensemble, be creative!. Write a function that given a training set does the following: </li>

        Created a validation set using 20% of the training set
        Trained each of your chosen classifiers on the training set
        Using the validation set created a new dataset where features are predictions made by each of your chosen classifiers
        Trained a logistic regression classifier to blend the predictions

