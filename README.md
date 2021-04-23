# Assignment Task-2 
Problem statement: 

* >Use this dataset to train a CNN. Use no other data source or pretrained networks, and explain your design choices during preprocessing, model building and training. Also, cite the sources you used to borrow techniques. A test set will be provided later to judge the performance of your classifier. Please save your model checkpoints.

* >Next, select only 0-9 training images from the above dataset, and use the pretrained network to train on MNIST dataset. Use the standard MNIST train and test splits. How does this pretrained network perform in comparison to a randomly initialized network in terms of convergence time, final accuracy and other possible training quality metrics? Do a thorough analysis. Please save your model checkpoints.

* >Finally, take the following dataset, train on this dataset and provide test accuracy on the MNIST test set, using the same test split from part 2. Train using scratch random initialization and using the pretrained network part 1. Do the same analysis as 2 and report what happens this time. Try and do qualitative analysis of what's different in this dataset. Please save your model checkpoints.

### Developing Environment
Everything was trained on Google colab with GPU support. You can run the notebooks by clicking on <a href="" target="_blank"> <img src="https://colab.research.google.com/assets/colab-badge.svg\" alt="colab" /> </a> button on the top of the ipynb notebook. 
Note if the notebook fails to open up, please use [notebook-viewer](https://nbviewer.jupyter.org), and paste the corresponding notebook link.

## Model Dictionary for Part2:

|      var_name     |                details               |
|:-----------------:|:------------------------------------:|
| modelA            | {0,1..9} classes from Part1          |
| modelB            | Scratch trained MNIST                |
| modelC            | MNIST training with modelA's weights |
| nModel_scratch    | scratch training on noise dataset    |
| nModel_pretrained | Noise training with modelA's weights |


### Bibiliography: 

* [Alexnet with Softmax](https://medium.com/analytics-vidhya/multi-class-image-classification-using-alexnet-deep-learning-network-implemented-in-keras-api-c9ae7bc4c05f)

* Various Stackoverflow answers
* Some codes were borrowed from Andrew's Ng Deep learning Specialization