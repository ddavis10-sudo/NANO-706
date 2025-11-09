For part one of the homework, I used a wine quality dataset to look at different wines and their quality. The first step is to load the libraries and the dataset to gain the information needed for the analysis. Once the data is loaded, the next step is to visualize it. In this specific plot, alcohol and malic acid were used for the plot to detect the quality.
<img width="2390" height="1488" alt="image" src="https://github.com/user-attachments/assets/99b0c933-59f9-4936-9bd6-f5007fd50900" />


After getting a visual of the data, it's important to standardize the features and split the data because it can rescale the features to avoid bias and improve the accuracy no matter how many times the model is ran. This dataset will be split 80/20, which represents 80% training and 20% testing.
<img width="1876" height="418" alt="image" src="https://github.com/user-attachments/assets/005099fe-3635-4f30-8877-198b8cf2b70c" />


Next it's time to train the SVM model, this predicts how well the model will perform, and then evaluate it. This helps classify accurate data and once the code is ran the accuracy resulted in 0.97 which is very close to 1.
<img width="1900" height="1334" alt="image" src="https://github.com/user-attachments/assets/260a6bdb-9df4-4ae6-9d43-64e55b9df56e" />


Now that the accuracy of the SVM model is given, next is the Decision Tree model. This model breaks down the directive that's used to predict the quality of wine. To generate this model, you would need to train the model, predict the results, calculate the accuracy, and visualize the data. The Decision Tree model has an accuracy of 0.94, which is accurate but less accurate compared to the svm model.
<img width="645" height="358" alt="image" src="https://github.com/user-attachments/assets/cce091d3-ab49-40b9-966b-685f2eb9bc8c" />
/>


The final model to train and test is the Logistic Regression model. This is important to use in the wine dataset because it pays attention to the chemical properties and their relationship with the outcome of the wine and its overall quality. Just like the other models, you have to train and predict the data, but with Logistic regression, you have to include the Decision tree model. After initializing and predicting the Decision tree model into the logistic regression model, then you calculate the accuracy of the Logistic regression model. The result of the accuracy is 0.98, which is the most accurate result out of all three models.
<img width="1930" height="1210" alt="image" src="https://github.com/user-attachments/assets/b46d6661-cde8-4d67-8f34-53eff0270f86" />



For part two of the homework, I used the MNIST dataset to be able to detect objects/pictures and use them as resources for deeper learning. There were three classifiers used to detect the accuracy which was Random Forest, MLP (Neural Network), and Logistic regression that was used in Part one. After coding each classifier, the results show the accuracy of each. MLP Neural network has the highest accuracy.
<img width="645" height="358" alt="image" src="https://github.com/user-attachments/assets/0a31a21f-798d-41d5-88f6-051023ae376f" />


The next step is using the YOLO model. The YOLO model is significant because this model is known for it's object detection in real time. Once you insert the picture used for detection, you insert it into the yolo model.
<img width="852" height="260" alt="Screenshot 2025-11-09 at 18 10 44" src="https://github.com/user-attachments/assets/9d84e8d1-1415-4697-a0b5-2ba11859d75b" />


After inserting the picture, you start coding to generate the detection box/boxes. In this process the coding is to create the detection box/boxes and draw bounding boxes around the object of interest. Once you draw the bounding box, it has to be saved and displayed with detections to show if it focused on the right object in the image.

![image_alt](https://github.com/SetturaM/NANO-706-HW-FINAL/blob/main/Screenshot%202025-10-30%20095455.png?raw=true)
Finally, the image is now displayed with the bounding box that has detected a stop sign  in the picture. From the previous coding, it tells you the color of the bounding box, which is purple. 
<img width="903" height="472" alt="Screenshot 2025-11-09 at 18 12 08" src="https://github.com/user-attachments/assets/5dffd0ee-efbb-4c95-845f-932f5c87948c" />


