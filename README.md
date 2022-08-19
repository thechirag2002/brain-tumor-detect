# brain-tumor-detect
Detection of Brain Tumor from Br35H Brain images dataset using Transfer Learning involving a Deep learning approach


## About the Issue 

One of the more severe disorders that affects both children and adults is a brain tumour. 85 to 90 percent of all primary Central Nervous System (CNS) malignancies are brain tumours. About 11,700 patients are given a brain tumour diagnosis each year. For those who have a malignant brain or CNS tumour, the 5-year survival rate is roughly 34% for males and 36% for women.

The amount of complexity in brain tumours and their characteristics makes a manual inspection susceptible to errors.
Machine learning and artificial intelligence (ML/AI)-based automated classification systems have consistently outperformed manual categorization in terms of accuracy. Therefore, offering a system that does detection and classification utilising Convolution-Neural Network (CNN), Artificial Neural Network (ANN), and Transfer-Learning (TL) will be beneficial to physicians all over the world.

## About Dataset
- Yes	The folder yes contains 1500 Brain MRI Images that are tumorous
- No	The folder no contains 1500 Brain MRI Images that are non-tumorous

This data can be found publically [here](https://www.kaggle.com/datasets/ahmedhamada0/brain-tumor-detection) on [Kaggle](https://www.kaggle.com/) 

![](https://github.com/thechirag2002/brain-tumor-detect/blob/e65bb1b69c9bf56724a381be84adcf7c4a835576/yes-no.png)

## Used Tecgnology and Methodolgy
### Transfer Learning
The reuse of a previously learned model on a new problem is known as transfer learning. It's particularly popular in deep learning right now since it can train deep neural networks with a small amount of data.

```
tensorflow.keras.applications.mobilenet.MobileNet 
```
> MobileNet model is a network model using depthwise separable convolution as its basic unit. Its depthwise separable convolution has two layers: depthwise convolution and point convolution

### Data Augmentation - ImageDataGenerator
```
tensorflow.keras.preprocessing.image.ImageDataGenerator
```
Data is then augmented using Image data generator and then model is trained over 3000 augmented images and then finally model is externally tested with an external dataset indicating the following results with corresponding training cycle.

![](https://github.com/thechirag2002/brain-tumor-detect/blob/e65bb1b69c9bf56724a381be84adcf7c4a835576/results-plots.png)

# Training results
![](https://github.com/thechirag2002/brain-tumor-detect/blob/e65bb1b69c9bf56724a381be84adcf7c4a835576/training-evaluation.png)

# Testing results
![](https://github.com/thechirag2002/brain-tumor-detect/blob/e65bb1b69c9bf56724a381be84adcf7c4a835576/test-eavluation.png)
