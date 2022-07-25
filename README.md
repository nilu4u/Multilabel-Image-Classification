# Multilabel-Image-Classification
The dataset used here is of fashion industry and it is imbalanced.

I have used oversampling method and class weight methods to handle imbalanced data. Before that an additional column is used to understand how much the data is imbalanced. This column is the weighted sum of attributes. Like 16*Attr1 + 8*Attr2 + 4*Attr3 + 2*Attr4. A histogram plot on this additional column is used to check if the data is imbalanced.
I have tried with several loss funstions like Categorical Crossentropy loss with logits and Sigmoid Cross Entropy with logits
I have used Resnet50 as the base architecture
F1 score has been used as metric
For image Augmentation: rotation, width and height shift, brightness, shear, zoom, channel shift, horizontal flip and rescale

# suggessions
Some other methods can be used for balancing data like under sampling 
Additional image augmentation techniques like colour jitter and random cropping can be used
Also the model is trined on very less number of Epochs which can be increased
The model can also be trained on several call backs with changing learning rate
