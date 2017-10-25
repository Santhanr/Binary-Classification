# Binary-Classification
################################DATASETS############################
Each dataset corresponds to a JSON file named as $dataset$.json. JSON is
a lightweight data-interchange format, similar to a dictionary. After loading a dataset, you can
access its training, validation, and test splits using the keys ‘train’, ‘valid’, and ‘test’, respectively.
For example, suppose we load mnist subset.json to the variable x. Then, x['train0'] refers to the training set of mnist subset. 
This set is a list with two elements: x['train'][0] containing the features
of size N (samples) ×D (dimension of features), and x['train'][1] containing the corresponding labels of size N.
Next we will describe each one of the three datasets in more detail.
• toydata1 includes 240 data instances with binary labels that are linearly separable. The
data is split into a training set and a test set. You can look up training and test sets in
toydata1.json with ['train'] and ['test'], respectively.
• toydata2 includes 240 data instances with binary labels that are not linearly separable. The
data is split into a training set and a test set. You can look up training and test sets in
toydata2.json with ['train'] and ['test'], respectively.
• mnist subset: MNIST is one of the most well-known datasets in computer vision, consisting
of images of handwritten digits from 0 to 9. We will be working with a subset of the official
version of MNIST. In particular, we randomly sample 700 images from each category and split
them into training, validation, and test sets, which can be reached in mnist subset.json via keys 
['train'], ['valid'] and ['test'], respectively.
################################ALGORITHM############################
• K-Nearest Neighbors
The standard agorithm is implemented using euclidean distance and the K among [1,3,5,7,9] that gives the 
best classification accuracy is found.
• Logistic Regression
The optimal parameters for logistic regression is found using gradient descent. The objective is the cross-entropy
function. At each iteration, the average gradients from all training samples is computed and the
parameters are updated using the chosen step size (or learning rate).
