# KNN Classification with Abalone dataset

Classification task – Predict ‘Rings’ from other features. Rings indicate the age of the fish.
This dataset contains information about physical measurements of abalone for predicting 'Rings' from other features. This project classifies the data with KNN classifier. 

The dataset taken from [link](https://archive.ics.uci.edu/ml/datasets/abalone).

### Built with

* Google Colab

### Libraries used 
* Pandas
* Numpy
* Matplotlib
* Seaborn
* Scikit-learn 

### Highlights
* Improving on KNN using method of weighted KNN
* Ablation study on Normalization


### What is being done?
1)	Loading the dataset and splitting into Train-Test set  <br>

2)	Normalization and training <br>

3)	Running the model using its default configuration on the test data <br>
    Looping over values of K. Finding best accuracy and K value <br>
    Plotting the graph of K values against Accuracies <br>

4)  Improving KNN using weighted KNN method using 3 schemas - Default, Manhattan and Euclidean	 <br>
    Plotting the graph of K vs Accuracy for all the 3 configurations with normalization <br>

5)	Ablation Study on Normalization <br>
    Performing Ablation study by removing the normalization step from the pipeline of preprocessing <br>
    Plot the above accuracies against the K values for all the three configurations (Without normalization) <br>

### Conclusion
*   Effect of normalization/ Standardization - The normalizarion does not make the classifier reach high accuracy for any of the tested values of k. This is applicable to both uniform KNN and weighted KNN. <br>
*   Without the normalization, as k increases and the neighbourhood size inresases, the performance lowers. This is not observed in the case of normalized data.<br>
*   For the differenct weighting schemes, the performance is not very different. <br>
*   The accuracy is overall low (below 30%). Hence it can be said that more complex models might be needed to classify well in this domain. <br>





