# Deep Learning and GPU Examples

[![SWAN](https://swan.web.cern.ch/sites/swan.web.cern.ch/files/pictures/open_in_swan.svg)](https://swan-k8s.cern.ch/user-redirect/download?projurl=https://github.com/cerndb/NotebooksExamples.git)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cerndb/NotebooksExamples)

This folder contains Jupyter notebook examples of common deep learning tools, running on GPU resources.  
To use GPU resources in [SWAN](https://swan.web.cern.ch/), you need to
 - open a ticket with the SWAN team to get access to GPU resources
 - use SWAN from  https://swan-k8s.cern.ch 
 - select a software stack with `GPU`
   - to get the latest version of the tools used here select the 'bleeding edge' software stack

Contact: Luca.Canali@cern.ch

## Getting started with Deep Learning
These notebooks implement a classifier for digit recognition using the MNIST dataset, it is a sort of "Hello World!" for Deep Learning.

* [MNIST with TensorFlow Keras](TensorFlow_Keras_MNIST.ipynb)
* [MNIST with PyTorch](PyTorch_MNIST.ipynb)
* [MNIST with Pytorch Lightning](PyTorch_Lightning_MNIST.ipynb)

## Deep Learning and basic Data pipelines
These notebooks provide examples of how to integrate Deep Learning frameworks with some basic data pipelines using Pandas to feed data into the DL training step.  
They implement a  Particle classifier using different DL frameworks. The data is stored in Parquet format, which is a columnar format that is very efficient for reading data,
it processed using Pandas, and then fed into the DL training step.
  
![][classifier_image]
  
* [TensorFlow classifier with data from Pandas](TensorFlow_Keras_HLF_with_Pandas_Parquet.ipynb)
* [Pytorch classifier with data from Pandas](PyTorch_HLF_with_Pandas_Parquet.ipynb)
* [Pytorch Lightning classifier with data from Pandas](PyTorch_Lightning_HLF_with_Pandas_Parquet.ipynb)
* [XGBoost classifier with data from Pandas](XGBoost_with_Pandas_Parquet.ipynb)

## More advanced Data pipelines
These examples show some more advanced data pipelines, useful for training with large data sets. They show how to use
the Petastorm library to read data from Parquet files with TensorFlow and PyTorch, and how to use the TFRecord format with TensorFlow.

* [TensorFLow and Petastorm](TensorFlow_Keras_HLF_with_Petastorm_Parquet.ipynb)
* [PyTorch and Petastorm](PyTorch_HLF_with_Petastorm_Parquet.ipynb)
* [TensorFlow with TFRecord](TensorFlow_Keras_HLF_with_TFRecord.ipynb)

[gallery_url]:https://cern.ch/swanserver/cgi-bin/go?projurl=https://github.com/cerndb/NotebooksExamples.git
[classifier_image]:https://github.com/cerndb/SparkDLTrigger/raw/master/Docs/Physics_use_case.png

## Additional complexity with models and data
These examples implement the same particle classifier as in the previous examples, but with a more complex model 
and bigger data set.  

* [Data in TFRecord, TensorFlow on GPU, GRU-based model](TensorFlow_Inclusive_Classifier_GRU_TFRecord.ipynb)
   - Description: This notebook showcases the training process for the Inclusive Particle Classifier model, 
     using data stored in TFRecord format.
   - TensorFlow is configured to run on a GPU, and a GRU-based model architecture is employed.
* [Data in TFRecord, TensorFlow on GPU, Transformer-based model](TensorFlow_Inclusive_Classifier_Transformer_TFRecord.ipynb)
   - Description: This notebook showcases the training process for the Inclusive Particle Classifier model,
     using data stored in TFRecord format.
   - TensorFlow is configured to run on a GPU, and a Transformer-based model architecture is employed.
