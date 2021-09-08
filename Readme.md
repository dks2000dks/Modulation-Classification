# Modulation-Classification
Classification of wireless signals using AutoML models. Understadning their effectiveness towrds adversarial-attacks.

## AutoML
- AutoML is used to generate models for classification of wireless signals. AutoKeras library is used creating AutoML for deep learning models.

## References
- [How to choose a neural network architecture? – A modulation classification example](https://ieeexplore.ieee.org/document/9221167)
- [Modulation Classification with Deep Learning](https://in.mathworks.com/help/deeplearning/ug/modulation-classification-with-deep-learning.html)
- [Convolutional Radio Modulation Recognition Networks](https://arxiv.org/pdf/1602.04105.pdf)
- [Fast Deep Learning for Automatic Modulation Classification](https://arxiv.org/pdf/1901.05850.pdf)
- [Improvements to Modulation Classification Techniques using Deep Learning](http://noiselab.ucsd.edu/ECE228/projects/Report/76Report.pdf)
- [Black-box Adversarial ML Attack on Modulation Classification](https://arxiv.org/pdf/1908.00635.pdf)

## RadioML Dataset
Dataset: RML2016.10a.tar.bz2
Source of Dataset: https://www.deepsig.ai/datasets
- All modulation schemes and SNRs of the RadioML dataset are considered for training and testing.

## Data
- RadioML Dataset is split into training and validation dataset with 20% of data for validation.

## Architectures
- AutoML Customised ResNet, AutoML Customised CLDNN, AutoML Customised CNN and AutoML Customised RNN.

## Training and Testing
- Models are trained and evaluated on training and validation datasets respectively.
- Performance is also validated on ResNet, CLDNN and Robust-CNN models from [Improvements to Modulation Classification Techniques using Deep Learning](http://noiselab.ucsd.edu/ECE228/projects/Report/76Report.pdf).

## Adversarial-Attacks
Transfer-Based Untargeted Adversarial Attacks are performed on AutoML Models.
### PGD-Attack
- Projected Gradient Descent(PGD) technique is used to generate the adversarial samples and suurogate model is **Robust-CNN** from [Improvements to Modulation Classification Techniques using Deep Learning](http://noiselab.ucsd.edu/ECE228/projects/Report/76Report.pdf).

### CW-Attack
- Carlini and Wagner(CW) technique is used to generate the adversarial samples and suurogate model is **Robust-CNN** from [Improvements to Modulation Classification Techniques using Deep Learning](http://noiselab.ucsd.edu/ECE228/projects/Report/76Report.pdf).
