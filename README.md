# DOG/CAT CNN CLASSIFIER WITH HYPERPARAMETER TUNING USING WEIGHTS & BIASES (W&B)
# **Introduction**
This report outlines the process of building and tuning a Convolutional Neural Network (CNN) 
classifier to distinguish between images of dogs and cats. The model was trained using TensorFlow 
and Keras, and hyperparameter tuning was performed using Weights & Biases (W&B) to optimize the 
model's performance.
# **Dataset**
The dataset used consists of images of dogs and cats, with separate directories for training and 
testing data. The data was loaded using TensorFlow's image_dataset_from_directory function.
• Image Loading: The dataset is loaded using tf.keras.utils.image_dataset_from_directory
from the specified directories for training and testing data

![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/79ceeda0-2a09-45d2-879a-95dd60041783)

# **Data Preprocessing**
![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/d3b6aaf1-1561-4417-b59e-f799d80ec37e)

# **Data Spliting**
![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/6f150bec-6074-4c99-b56f-457e0231e8ce)

![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/b87ac060-7467-4346-b6cf-fd52a9f86a33)

# **Model Architecture**
![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/fe1b7dc2-e742-4ff1-b35b-7af70a275550)

# **Analysis**
![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/08648a04-7dd5-40ca-bf6c-1f5eae373c13)

# **Evaluation**

![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/44835634-0d57-4970-a9ee-908743b99110)

![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/c3744dad-128b-4bfb-9cad-17584cdc7d5c)

# **Hyperparameter tunning**
To Imporove Model we need to do **Hyperparameter tunning** with W&B

- first setup the W&B 
- Then set sweep configuartion
- train the model again
- find good parameter using W&B graphs
  ![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/0363bcca-b6be-4459-b420-59eb0b110d5a)

# **Try with different optimizers**
- Based on the training results for each optimizer, we can compare their performance in terms of accuracy and loss for both training and validation datasets. Here is a summary of the final epoch results for each optimizer:
  
| Optimizer        | Training Loss | Training Accuracy | Validation Loss | Validation Accuracy |
|------------------|---------------|-------------------|-----------------|---------------------|
| SGD              | 0.6917        | 0.5642            | 0.6933          | 0.5000              |
| SGD with Momentum| 0.6909        | 0.5312            | 0.6859          | 0.6081              |
| RMSProp          | 0.4287        | 0.8212            | 0.4000          | 0.8514              |
| Adagrad          | 0.3873        | 0.8420            | 0.3858          | 0.8243              |
| Adam             | 0.0439        | 0.9931            | 0.0217          | 1.0000              |

# Conclusion

Based on the results obtained from the hyperparameter tuning experiments, the Adam optimizer emerges as the most suitable choice for the task at hand. It consistently outperformed other optimizers in terms of both training and validation metrics, showcasing superior convergence properties and accuracy.

## Optimizer Comparison Summary

- **Training Accuracy Curves:** Adam demonstrated the fastest and highest increase in accuracy during training.
- **Validation Accuracy Curves:** Adam consistently maintained the highest validation accuracy throughout the training process.
- **Training Loss Curves:** Adam exhibited the fastest decrease in loss during training epochs.
- **Validation Loss Curves:** Adam consistently maintained the lowest validation loss among all optimizers.

Overall, Adam's adaptive learning rate and momentum combination make it exceptionally effective for training deep learning models, leading to improved performance and convergence.

![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/a641dd91-bfd9-47a7-aa23-b9ebf7248489)

The visual summary above further reinforces the superiority of Adam as the optimizer of choice for this task.

# **Model Prediction**

- using with hyperparameter and adam optimizer model was trained well and test the model test results shown below:
![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/0bd2aced-3ec2-496f-b773-f6d1d76300f6)

![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/4832f4f8-bdfe-42f3-bcef-0e3901aed0cb)

# **Create a Web page for identify the image whether dog / cat**

![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/43f9fe6b-c2db-4e74-887b-607a3e7188d7)
![image](https://github.com/Priya-Sivalingam/Deep-Learning-Projects/assets/112175724/665046cd-f9ef-4d7f-ab50-eee5fb9ba966)






