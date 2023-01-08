# Principal-componant-analysis

For this demonstration, we begin with a very popular machine learning dataset - 'Iris'. In the next few segments, you will learn the necessary steps needed to perform PCA on a dataset and then appreciate how it helps in visualising your data that contains more than two dimensions.
steps that you've performed in the video and something that you should do whenever you perform PCA on any other dataset as well.

 

1. After basic data cleaning procedures, standardise your data

 

2. Once standardisation has been done, you can go ahead and perform PCA on the dataset. For doing this you import the necessary libraries from sklearn.decomposition.

 

from sklearn.decomposition import PCA
 

3. Instantiate the PCA function and set the random state to some specific number so that you get the same result every time you execute that code. (If you want to learn more about random state and how it works, you can check this StackOverflow answer)

 

pca = PCA(random_state=42)
 

4.  Perform PCA on the dataset by using the pca.fit function. 

 

pca.fit(x)
 

 

5. The Principal Components can be accessed using the following code:

 

pca.components_
 

Executing the above code will give the list of Principal components of the original dataset. They'll be of the same number as the original variables in your dataset.
