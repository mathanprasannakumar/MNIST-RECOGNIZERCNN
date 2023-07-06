# MNIST-RECOGNIZER-CNN
***Here i implemented a CNN model which will recognize the MNIST handwritten data set with a accuracy of 99.67 %***

<h4>1) Dataset </h4>
<ul>
  <li>The mnist dataset is loaded using keras API datasets</li>
  <li><b>Preprocessing the dataset</b></li>
  <ul>
    <li>converting to a single channel image</li>
    <li>applied one hot encoding to the label values </li>
    <li>normalizing the pixel values to be in the range of 0 to 1</li>
    <li>Chaninging the datatype of the pixel to float 32</li>
  </ul>
</ul>

<h4>2) Model architecture </h4>
<ul>
  <li>Sequentail api is used</li>
  <li>single Convolution and Flattern layers is added </li>
  <li>Batch normalization is applied after convolution and flatten layer</li>
</ul>

<h4>3) Model configuration</h4>
<ul>
  <li>SGD optimizer is used</li>
  <li>lost: Categorical cross entropy</li>
  <li>The model will be evaluated using five-fold cross-validation. The value of k=5 was chosen to provide a baseline for both repeated evaluation and to not be so large as to require a long running time. Each test set will be 20% of the training dataset, or about 12,000 examples, close to the size of the actual test set for this problem.</li>
</ul>
