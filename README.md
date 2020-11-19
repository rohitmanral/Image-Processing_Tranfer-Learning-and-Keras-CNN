# Image-Processing_Tranfer-Learning-and-Keras-CNN

# Specification
## Performing the following tasks:

## Building a Small CNN from Scratch
Building two versions.

Both versions have two conv layers and two max pooling layers in your CNN.  One version contains dropout layers and the other does not not.  You can decide other aspects of the architecture.  Briefly explaining what decisions made. 

Trained both versions of the CNN on the Caltech-101 dataset, leaving out the 5 largest categories, as is done in the Colab tutorial.

Determined the accuracy on my test data for each version of the network, and discussed any differences.

## Applying Transfer Learning to a Pretrained Network
Loaded a pretrained network (ResNet-50) & accessed this via keras pretrained models.  Apparently there are a few issues with the initial implementation in Keras, so I'd recommend you use ResNet50V2 instead (i.e. keras.applications.ResNet50V2).

Adapted the model to the Caltech-101 dataset, and retrained.  For my first retraining, I kept all layers frozen except the last one.  The retrain again, unfreezing one extra layer.  Compared the accuracies of these two retrained models with each other, and also with the CNNs built from scratch above.

## Applying Data Augmentation to a Pretrained Network
Retrained my ResNet-50 model again, this time including some data augmentation.  Explaining what kinds of data augmentation I have chosen and why, and compared the results with those above.

Note that if you're doing this in Colab, and you only have the minimum RAM, you may not be able to run this for very many epochs.  You can increase the RAM to 25Gb.  (When your program crashes because you've run out of memory, you get the option of rerunning with memory increased to this maximum.  Alternatively, you can force this.  On the other hand, you might just have 25Gb from the start; that's the case for me, although I don't know why.)
