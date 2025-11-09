For part one of the homework, I used a wine quality dataset to look at different wines and their quality. The first step is to load the libraries and the dataset to gain the information needed for the analysis. Once the data is loaded, the next step is to visualize it. In this specific plot, alcohol and malic acid were used for the plot to detect the quality.
![image alt](https://github.com/SetturaM/NANO-706-HW-FINAL/blob/main/Screenshot%202025-10-30%20092314.png?raw=true)

After getting a visual of the data, it's important to standardize the features and split the data because it can rescale the features to avoid bias and improve the accuracy no matter how many times the model is ran. This dataset will be split 80/20, which represents 80% training and 20% testing.
![image alt](https://github.com/SetturaM/NANO-706-HW-FINAL/blob/main/Screenshot%202025-10-30%20092631.png?raw=true)

Next it's time to train the SVM model, this predicts how well the model will perform, and then evaluate it. This helps classify accurate data and once the code is ran the accuracy resulted in 0.97 which is very close to 1.
![image a;t](https://github.com/SetturaM/NANO-706-HW-FINAL/blob/main/Screenshot%202025-10-30%20092719.png?raw=true)

Now that the accuracy of the SVM model is given, next is the Decision Tree model. This model breaks down the directive that's used to predict the quality of wine. To generate this model, you would need to train the model, predict the results, calculate the accuracy, and visualize the data. The Decision Tree model has an accuracy of 0.94, which is accurate but less accurate compared to the svm model.
![image alt](https://github.com/SetturaM/NANO-706-HW-FINAL/blob/main/Screenshot%202025-10-30%20092944.png?raw=true)

The final model to train and test is the Logistic Regression model. This is important to use in the wine dataset because it pays attention to the chemical properties and its relationship with the outcome of the wine and it's overall quality. Just like the other models, you have to train and predict the data, but with Logistic regression you have to include the Decision tree model. After initializing and predicting the Decision tree model into the logistic regression model, then you calculate the accuracy of the Logistic regression model. The result of the accuracy is 1.00, which is the most accurate result out of all three models.
![image_alt](https://github.com/SetturaM/NANO-706-HW-FINAL/blob/main/Screenshot%202025-10-30%20093046.png?raw=true)


For part two of the homework, I used the MNIST dataset to be able to detect objects/pictures and use them as resources for deeper learning. There were three classifiers used to detect the accuracy which was Random Forest, MLP (Neural Network), and Logistic regression that was used in Part one. After coding each classifier, the results show the accuracy of each. MLP Neural network has the highest accuracy at 97.86%, following at 96.75% is Random Forest, and lastly Logistic Regression has an accuracy of 92.02%.
![image_alt](https://github.com/SetturaM/NANO-706-HW-FINAL/blob/main/Screenshot%202025-10-30%20093534.png?raw=true)

The next step is using the YOLO model. The YOLO model is significant because this model is known for it's object detection in real time. Once you insert the picture used for detection, you insert it into the yolo model.
![image_alt](https://github.com/SetturaM/NANO-706-HW-FINAL/blob/main/Screenshot%202025-10-30%20095826.png?raw=true)

After inserting the picture, you start coding to generate the detection box/boxes. In this process the coding is to create the detection box/boxes and draw bounding boxes around the object of interest. Once you draw the bounding box, it has to be saved and displayed with detections to show if it focused on the right object in the image.

![image_alt](https://github.com/SetturaM/NANO-706-HW-FINAL/blob/main/Screenshot%202025-10-30%20095455.png?raw=true)
Finally, the image is now displayed with the bounding box that has detected my face in the picture. From the previous coding, it tells you the color of the bounding box, which is green. This shows that in that bounding box there is no other detectable objects other than my face.

![image_alt](https://github.com/SetturaM/NANO-706-HW-FINAL/blob/main/Screenshot%202025-10-30%20095505.png?raw=true)
