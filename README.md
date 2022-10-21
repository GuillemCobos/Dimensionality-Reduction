# Dimensionality-Reduction
We use principal component analysis to reduce the number of variables that need to be fed into a classification algortihm for cancerigenous tumors. 
We use supervised learning techniques on a dataset containing 30 features describing a tumor on 569 patients, together with a label describing whether the tumor is benign/malign. 

The code follows the structure:

First Part. A classification algorithm is trained using the original 30 features describing a tumor. We use a decision tree algorithm provided by the library sklean to do the job. We assess its accuracy using standard train/test splitting and predifined functions.

Second Part. We perform a principal component analysis on the data, and only retain the first 2 principal components. With these only 2 features we now train a similar decision tree classification algorithm. Accuracy levels similar to the original model that used 30 variables are obtained, even though we have reduced the number of input variables from 30 to 2!
