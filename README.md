Instructions:

Let's optimize the decision tree, this process is called hyperparameter tuning. In lieu of manually selecting values to optimize the decision tree e.g. max_depth and criterion, we will use random search to estimate the values. The decision tree has many parameters, but let's focus on optimizing criterion, max_depth and min_samples_split.

Perform the following steps:

Manually review the results from the previous exercise. Do you notice any evidence of overfitting or underfitting?

Extract the following features that will be used to build the model: 'VendorID', 'RatecodeID', 'PULocationID', 'DOLocationID', 'passenger_count', 'trip_distance', 'fare_amount', 'extra', 'mta_tax', 'tolls_amount', 'improvement_surcharge', 'total_amount', 'trip_type', 'congestion_surcharge', 'tip'

Note: The column 'tip' contains the labels (i.e. the predicted output). The labels are: no-tip, low, standard or good.
Split the dataset into a training set and a test set; The test set should comprise 30% of the dataset. Ensure the data is randomized and that stratified samples are obtained. Scikit-learn has a module that is useful to split the data according to this criteria.

Instantiate the Decision Tree Classifier (do not assign values for any parameters)

Create a dictionary that contains the parameters from the decision tree that should be optimized: criterion, max_depth and min_samples_split.

Perform a random search to identify suitable values for the selected parameters. The method in scikit-learn is called RandomizedSearchCV.

Train the decision tree using the suggested parameters from the random search.

Evaluate the accuracy.

Visualize the decision tree.

Inspect the visualization and summarize the results using 2-5 sentences. Do you notice any improvements and did the tree develop better rules to split the data. Did this exercise address any overfitting or underfitting that occurred in the previous exercise.

You may reuse code snippets from the previous exercise (where applicable).

If you have any questions about the assignment, create a GitHub issue and @mention the instructor.

NOTE: The jupyter notebook DecisionTreePt2.ipynb contains starter code. Follow the instructions in each step. Also read the python comments which contain additional information. Comments that are prefaced by TODO: require that you either provide a value or line of code. You may use the starter code, or create your own script from scratch.
