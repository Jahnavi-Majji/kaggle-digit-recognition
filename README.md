# kaggle-digit-recognition

MNIST is the de facto “hello world” dataset of computer vision. In this competition, our goal is to correctly identify digits from a dataset of handwritten images.
In this competetion, our goal is to build a model that identifies the hand-written digits correctly. The dataset consists of 42,000 images in the training set and 28,000 images in the test set.

Download the dataset [here](https://www.kaggle.com/c/digit-recognizer/data)
***
I used 2 CNN models with different architecture. 

The first model follows the pattern of VGG16 architecture. 

The second follows the Le-Net5 architecture with regularization, batch normalization, dropout. 
The architecture and their corresponding results are mentioned below
#
#### Model1 architecture
(Conv2D => Conv2D --> BatchNorm => MaxPooling => Dropout) *2 => Flatten => (Fully Connected => BatchNorm) *3 => Dropout => Output

#### Model2 architecture
(Conv2D => Conv2D => MaxPooling => Dropout ) *2 => Flatten => Fully connected layer => => Dropout => Output
___

#### Results
#
ST | LeNet5Model |
---|--------
Total params | 390,562
Trainable params | 389,434
Non-trainable params | 1,128
Epochs trained | 30
Loss | 0.0184
Training set accuracy | 99.62
val_loss | 0.236
val_accuracy | 99.33 


#### References

* [Yassine Ghouzam](https://www.kaggle.com/yassineghouzam/introduction-to-cnn-keras-0-997-top-6)
* [Taavish Thaman](https://github.com/TaavishThaman/LeNet-5-with-Keras)
