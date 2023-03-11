This project aims to detect facial expressions using facial point detection. The project consists of two datasets: data.csv and icml_face_data.csv. The first dataset contains the X and Y coordinates of various facial points, such as eyes, nose, and mouth, for different people. The second dataset is the ICML Face Data CSV, which can be downloaded from https://figshare.com/articles/dataset/icml_face_data_csv/19792891/1.

**Data Augmentation**

Before building the models, we performed data augmentation on both datasets. Data augmentation involved inverting the X and Y axis, increasing and decreasing the brightness of the images, and more. The purpose of data augmentation is to increase the size and diversity of the dataset, which can lead to better performance of the models.

**ResNET Model**

We built a ResNET model for the data.csv dataset and saved the model as a JSON file. ResNET is a deep learning architecture that has been shown to perform well on image classification tasks. We chose this architecture because it is known to be effective at learning complex features from images.

**CNN Model**

We built a CNN model for the icml_face_data.csv dataset and saved the model as a JSON file. CNN is another deep learning architecture that is commonly used for image classification tasks. We chose this architecture because it is well suited for processing image data.

**Combining Models**

After building both models, we combined them to predict the emotion of people in the dataset. We used the trained models to detect facial points in images and then fed these points to the models to predict the corresponding emotion.

**Conclusion**

This project demonstrates how facial expression detection can be achieved by detecting facial points using deep learning techniques. The combination of ResNET and CNN models can lead to accurate predictions of emotions. The code and dataset used in this project can be found in this GitHub repository.
