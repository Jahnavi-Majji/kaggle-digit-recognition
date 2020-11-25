# kaggle-digit-recognition

MNIST is the de facto “hello world” dataset of computer vision. In this competition, our goal is to correctly identify digits from a dataset of handwritten images.
In this competetion, our goal is to build a model that identifies the hand-written digits correctly. The dataset consists of 42,000 images in the training set and 28,000 images in the test set.

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
. | Model 1 | Model2
---|--------|-------
Total params | 887,530 | 715,850
Trainable params | 887,530 | 714,762
Non-trainable params | 0 | 1,088
Epochs trained | 30 | 30
Loss | .  |  .
Training set accuracy |  .. | ..
val_loss | ... | ...
val_accuracy | ... | ...
