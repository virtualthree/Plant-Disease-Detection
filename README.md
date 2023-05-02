# Plant-Disease-Detection

This paper is based on disease detection in Maize and Tomato leaves using hybrid Deep Learning acrhitectures and Nature Inspired Algorithms. We classify the disease using various Machine Learning classifiers.

Image Preprocessing
The photos must be of a small size to ensure that there aren't too many features when feeding them into a neural network. Also the images can be of different size. Thus, to make them of the same size, we resize the images to pixel values 224x224x3 which gives us 1,50,528 parameters, which is still manageable as compared to images of large pixel values.

Feature Extraction:
The method of feature extraction is covered in this section. The feature extraction process makes use of four deep learning models. In this work, pre-trained versions of MobileNetv2, DenseNet121, VGG16, and Resnet50 are used. Deep Transfer Learning is used to retrain both models on a more prominent maize disease cases (DTL) dataset. The idea of transfer learning is graphically represented in Figure3. By applying the knowledge gained from large and well-known datasets, transfer learning enables tiny datasets to perform better. Features are retrieved using both MobilneNetv2 and DenseNet121 to increase classification accuracy. Another approach to feature extraction that makes use of both VGG16 and ResNet50 operates in a similar manner. The combined deep learning architectures' retrieved features are later mixed and sent to the classifiers.

Feature Selection:
Feature selection is a crucial step in enhancing accuracy and calculation speed. It becomes necessary when the initial feature set is relatively large since processing the feature set calls for additional processing power. The literature presents a wide range of feature selection strategies. In this study, noteworthy features are extracted from the initial feature set using feature selection. The computational time is shortened by processing the notable features from the initial feature collection. In the proposed work, namely, 4 nature inspired algorithms are used for feature selection. Those are:
1. Whale Optimization Algorithm
2. Particle Swarm Optimization
3. Harris Hawk Optimization
4. Jaya ALgorithm

Machine Learning Classifiers:
After extracting features using the combinations of MobileNet and DenseNet and VGG and ResNet, the feature set is split in training and testing data and then passed to the machine learing classifiers for getting various metrics mentioned in the results section.The machine learning models used are Random Forest classifier, SVM Classifier and Ada Boost Classifier.
