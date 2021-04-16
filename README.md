<h1>Image Recognition on CIFAR-10 dataset</h1>

<h2>Dataset</h2>

<p>The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.</p>

<p>The dataset is divided into five training batches and one test batch, each with 10000 images. The test batch contains exactly 1000 randomly-selected images from each class. The training batches contain the remaining images in random order, but some training batches may contain more images from one class than another. Between them, the training batches contain exactly 5000 images from each class.</p>

<p>Each image in the dataset belongs to one of the following classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck.</p>

<p>The classes are completely mutually exclusive. There is no overlap between automobiles and trucks. "Automobile" includes sedans, SUVs, things of that sort. "Truck" includes only big trucks. Neither includes pickup trucks.</p>

<p>The dataset can be downloaded <a href="https://www.cs.toronto.edu/~kriz/cifar.html">here</a>.</p>

<h2>Training</h2>

<h3>Libraries used</h3>

<ol>
<li>NumPy</li>
<li>Tensorflow</li>
<li>Matplotlib</li>
</ol>

<h3>Model</h3>

<p>A Convolutional Neural Network from keras was used to train the model. The major features of the network architecture consisted of one convolutional layer, one hidden layer, and one output layer. Categorical Cross-Entropy was used as the loss function, while taking accuracy as a metric. Early Stopping was also implemented during training, to mostly avoid overfitting.</p>

<p>A total of 40,000 images were used for training, another 10,0000 images were used for evaluation, and then 1,000 images were used for testing.</p>

<h2>Evaluation</h2>

<p>After the trainig was done, the model was able to produce an accuracy of 96.69% on the test set, 60.35% on the validation set, and 59.36% on the test set.

<h2>Repository</h2>

<p>In this repository, the code for the training can be found in train.ipynb file, the model folder contains the already saved model from the training.</p>