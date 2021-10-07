# Classification-with-Health-Records


Dataset Description
This dataset includes information about over 100,000 medical appointments of different patients from different neighborhoods in Brazil, and this dataset discuss very important point that why a person makes a doctor appointment, receives all the instructions and no-show. 


<h3>Part I: Data prep:</h3>


<ul> This includes: </ul>

<li>Reading in data csv file </li>

<li>Cleanup data column names </li>

<li>Remove records with erroneous entries (e.g., negative ages, look at what people have done in Kaggle) </li>

<li>Create a test set of 20k records that you won’t touch again for the reminder of this project until Part III. Use stratified sampling on the No-show variable to ensure test set and training set class proportions are the same. Save the train and test sets as csv files in the processed_data directory. </li>

<li>Plot the No-show variable against the other variables in the dataset as part of Exploratory Data Analysis </li>

<li>Create a preprocessing pipeline using scikit to prepare the data for the ML algorithms we will use. At a minimum, standardize numerical variables, transform categorical variables into one or more numerical values. You may apply other transformations that you think would be useful (e.g., logarithmic transformations).</li>



