<h2>Aim</h2>

In this notebook, a Convolutional Neural Network (CNN) has been developed for the purpose of facial expression recognition. The primary objective of this study is to accurately classify facial images into one of the seven predefined categories of facial emotions. The CNN models have been trained using gray-scale photos obtained from the Kaggle platform, with varying depths to explore the impact on performance. To mitigate the issue of overfitting, several techniques such as dropout, batch normalization, and regularization have been employed. The main focus of this study is to enhance the performance of convolutional neural network models. Finally, the performances of all three CNN models are compared, and the accuracy and loss visualizations are presented to gain better insights and understanding of the models' capabilities.

<h2>Datasets</h2>
For this experiment, [Kaggle FER-2013 Dataset](https://www.kaggle.com/datasets/robikscube/hourly-energy-consumption) has been used which consists of more than 35,000 well
structured grayscale 48×48 pixel pictures of faces expressing a range of emotions and Seven categories have been created based on these facial expressions - 
happy, disgust, fear, happiness, sadness, neutral and angry.



<img width="474" alt="Screenshot 2023-06-09 at 3 19 17 AM" src="https://github.com/tiashamondal29/Facial-emotion-recognition-using-CNN/assets/62413982/36c67341-9664-432c-819d-3d333255b7c3">


<h2>Methodology</h2>
Initially, a shallow CNN Model was constructed, comprising two convolutional layers and one fully connected (FC) layer. However, experimental results indicated that this model suffered from overfitting, whereby it performed well on the training data but failed to generalize effectively to unseen data.

To address the overfitting issue, an improved CNN Model was devised. This enhanced model incorporated rectified linear unit (RELU) activation function, followed by max pooling with a kernel size of (2,2). By incorporating these modifications, the overfitting problem was alleviated to a certain extent, leading to improved performance on unseen data.

Moreover, to further enhance the model's performance, a deep CNN Model was developed. This augmented model included additional convolutional layers and dropout layers. The increased depth of the network and the integration of dropout layers helped mitigate overfitting and improved the model's ability to capture complex features and patterns in the facial expression data.

Through these iterations and modifications, the CNN models were progressively refined to achieve better performance and generalization capabilities for facial expression recognition.


<h2> Results and Comparision </h2>

**1. The accuracy and the loss function of train and validation data for different number of iterations of shallow model**
<img width="1018" alt="Screenshot 2023-06-09 at 3 27 57 AM" src="https://github.com/tiashamondal29/Facial-emotion-recognition-using-CNN/assets/62413982/3a067b42-7995-4cee-8892-f8bc46e7c00e">


**2.The accuracy and the loss function of train and validation data for different number of iterations of the improved CCN Model**

<img width="1018" alt="Screenshot 2023-06-09 at 3 28 55 AM" src="https://github.com/tiashamondal29/Facial-emotion-recognition-using-CNN/assets/62413982/a7dff8cc-16b8-4d17-8388-6da7cd8d8439">


**3. The accuracy and the loss function of train and validation data for different number of iterations of the Deep CCN Model after Hyterparameter Tuning**


<img width="1018" alt="Screenshot 2023-06-09 at 3 29 57 AM" src="https://github.com/tiashamondal29/Facial-emotion-recognition-using-CNN/assets/62413982/c570817c-6590-4a40-b601-eb004f77edcd">


<h2>A Comparision Study</h2>
<img width="1059" alt="Screenshot 2023-06-09 at 3 30 32 AM" src="https://github.com/tiashamondal29/Facial-emotion-recognition-using-CNN/assets/62413982/86fdb107-c0d1-468b-a987-de9bfad964c6">


<h2>Conclusion</h2>
In conclusion, this study demonstrated that deep CNN models have the ability to learn facial features and improve facial expression recognition. Despite a slight reduction in accuracy, these models effectively addressed the overfitting issue, enhancing their generalization capabilities. Further research can explore additional techniques to optimize performance in this area.
