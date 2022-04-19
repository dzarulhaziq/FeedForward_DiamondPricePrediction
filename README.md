# Diamond Price Prediction Using Feedforward Neural Network

## 1. Summary

### The dataset use to perform this prediction can be obtain [here](https://www.kaggle.com/datasets/shivam2503/diamonds)
### The goal of this network is to perform prediction on the diamond prices based on several features :
- 4C (cut,clarity,color,carat)
- dimensions (x,y,z)
- depth
- table

## 2. IDE and Framework

### The project is created using google colaboratory as the main IDE.
### The frameworks used in the project are as listed below:
- Pandas
- Numpy
- Scikit-learn
- TensorFlow Keras

## 3. Methodology

### 3.1 Data Pipeline
The data is first loaded and preprocessed, such that unwanted features are removed. Categorical features are encoded ordinally. Then the data is split into train-validation-test sets, with a ratio of 60:20:20.

### 3.2 Model Pipeline
A feedforward neural network is constructed that is catered for regression problem. The structure of the model is fairly simple. Figure below shows the structure of the model.

![image](https://user-images.githubusercontent.com/103733709/164048086-cc6d0301-9abe-44d4-9399-e97942e407ad.png)

The model is trained with a batch size of 64 and for 100 epochs.The training MAE of 571.3531 and validation MAE of 347.9800. The two figures below show the graph of the training process, indicating the convergence of model training.

![image](https://user-images.githubusercontent.com/103733709/164047732-0c85fe07-61b2-4947-8362-a0f9a327b829.png)

## 4. Results
The model are tested with test data. The evaluation result is shown in figure below.
![image](https://user-images.githubusercontent.com/103733709/164047808-0e37d26a-3fd8-402d-8ef3-646a78251dc2.png)

The model is also used to made prediction with test data. A graph of prediction vs label is plotted, as shown in the image below.
![image](https://user-images.githubusercontent.com/103733709/164047918-d79d1c01-39b0-43b4-b3d8-e709b7a86d41.png)

Based on the graph, a clear trendline of y=x can be seen, indicating the predictions are fairly similar as labels. However, several outliers can be seen in the graph.
