# Image Classification with Tensorflow CNN

### 1.0 Project Summary
___

| Project | Findings | Key Feature | Data Source |
|---|---|---|---|
| [Dog Breed Multi-classification](https://github.com/86lekwenshiung/Multiclass-Image-Classification-with-CNN-in-Tensorflow/raw/main/Dog_Vision_Dog_Breed_Multiclassification.ipynb) | [Summary](#section_2) | * Tensorflow<br>* Transfer Learning<br>* Convolutional Neural Network(CNN)<br>* mobilenet_V2 | [Kaggle Dataset for Dog Breeds](https://www.kaggle.com/c/dog-breed-identification/data) |
| Food 101 Multi-classification | Summary | * Tensorflow<br>* Transfer Learning<br>* Convolutional Neural Network(CNN)<br>* Efficientnet_B0 | 101 Food Images |

<a id = 'section_2'><a/>
### 2.0 Findings for Dog Breed Multi-classification
___

Using pre-trained model from mobilenet_v2 (tensorflow hub) to train our model to identify ~ 120 dog breeds. Using a small data set of 1000 images to pre-trained our model , the model is observed to be very overfitted with a validation accuracy of 60% compared to a training accuracy of nearly 100%.

  * Training Data : 800,
  * Validation Data : 200
  <p align = 'center'>
  <img src = 'https://raw.githubusercontent.com/86lekwenshiung/Multiclass-Classification-with-CNN-in-Tensorflow/main/images/baseline.png'>
    <p/>
  
  Using the same sequence , we increases the datasize to the full dataset of 10,000 images. The model performed much better , but it is obersved to be overfitted with a training accuracy of 81%.
  * Training Data : 8177,
  * Validation Data : 2045
  * Next Step : Further fine tuning layers could be added in the image preprocessing such as `data augmentation` and `fine tuning` the trainable layers.
  <p align = 'center'>
  <img src = 'https://raw.githubusercontent.com/86lekwenshiung/Multiclass-Classification-with-CNN-in-Tensorflow/main/images/fulldata.png'>
    <p/>
 
  Below image is a way we could visualize how well our model predict against the images ; The images where they performed well and not so well.
<img src = 'https://raw.githubusercontent.com/86lekwenshiung/Multiclass-Classification-with-CNN-in-Tensorflow/main/images/prediction_summary.PNG'>
