MNIST Dataset

A generalization of multi-label classification where each label can be multiclass (i.e., it can have more than two possible values). I build a system that removes noise from images. It will take as input a noisy digit image, and it will output a clean digit image, represented as an array of pixel intensities, just like the MNIST images.

I cleaned the image using KNN classifier. It is an example of Multioutput classification. A single label is Multilabel as it has 784 classes and each of the 784 pixel can have values from 0 to 255, hence it is a Multioutput classification example.
