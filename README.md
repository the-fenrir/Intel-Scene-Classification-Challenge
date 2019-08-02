# Intel-Scene-Classification-Challenge

Contains my codes which was used in the Intel Scene Classification Challenge

Various CNN Architectures were used. Validation Accuracy of Various Models are as follows:
 - Inception ResNet V2: 92.4 %
 - Inception V3: 92.2 %
 - ResNet 50: 92.5 %
 - Xception Net: 94.2 %
  
Basically, My idea was based on first initialising the initial layers with pretrained weights and freezing them to prevent any backprop, and adding certain more layers on top of them which would learn from the features extracted by the initial layers.
After reaching, a plateau in the learning curve, the initial layers were unfrozen.
This basically helped in the fine tuning of the features of the initial layers without much radical change in them.

The above method proved to work better for all the tried architectures except ResNet50.

And the Models were trained on Kaggle Kernels and CNN Architectures were imported from the Keras Libraries which were then trained with a Tensorflow Backend.
