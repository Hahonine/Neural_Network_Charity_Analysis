# Neural_Network_Charity_Analysis

## Results

- The target variable is the "Is successful" metric listed in the dataset for each datapoint.

- Every other metric except identifiers (name and EIN), including Classification, Income, Request type, and several others, are all features of the model used to predict the target variable.

- Identifiers (in this case, company name and EIN) were removed from the dataset for irrelevence to the model results.

## Compiling, Training, and Evaluating the Model
- The neural network model utilized 2 input layers with 160 and 90 neurons respectively, activated with the 'ReLu' activation function. One output layer with a single neuron utilizing the 'Sigmoid' activation function was also included in the model.

- I was unable to optimize the model despite adjusting the optimization algorith, the neuron count, and even pruning some less relevant data from the process dataset. My peak accuracy was with the original unoptimized model at roughly 73.6% accuracy.

## Summary
- All in all, the model did a sufficient job predicting the risk of loaning money to an entity with specified traits. While not perfectly accurate, the results are close.

- Due to the widespread Classifications included in the dataset and the binary result being known for the entire dataset, a supervised Machine Learning function such as a Logistical regression with linear scaling of the features might produce a more accurate result. To use a supervised ML in this way, it is recommended to scatter plot the data with a color code equal to the result for each datapoint, and pick the function based on the observed shape of the data.