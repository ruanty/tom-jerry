# Tom and Jerry Classification
<img width=270 src="img/jerry.jpg"> <img width=270 src="img/tom.jpg"> <img width=270 src="img/dogs.jpg">       

### 🚀 Goal
Find Tom and Jerry in images with Convolutional Neural Network.
Since Tom and Jerry are in radically different shapes in different frames, we applied different models to find the best approaches. 

### 🗃 [Data](https://www.kaggle.com/datasets/balabaskar/tom-and-jerry-image-classification?select=ground_truth.csv)
This dataset contains 5478 images extracted from some of Tom & Jerry's show videos. Each image is labeled with "Tom only", "Jerry only", "Tom and Jerry", or "No Tom or Jerry". 

Credit: [Kaggle: Bala Baskar](https://www.kaggle.com/balabaskar)

### Approach 1:
We built 2 seperate binary classifers for Tom and Jerry individually, and we trained each model for 10 epochs. 
The Tom model produces a train accuracy of 99% and a validation accuracy of 93%. 
The Jerry model produces a train accuracy of 99% and a validation accuracy of 91%. 

<img width=350 src="img/tom_model.png">    <img width=340 src="img/jerry_model.png">

### Approach 2:
We labelled each image with one of the 4 labels:
* No Tom or Jerry = 0
* Tom only = 1
* Jerry only = 2
* Tom and Jerry = 3

We built a multi-class classifer for this setting, and we trained each model for 10 epochs. 
The model produces a train accuracy of 97% and a validation accuracy of 80%. 

<img width=340 src="img/combined_model.png">    
