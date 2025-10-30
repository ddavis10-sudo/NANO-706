# Assignment 2
This assignment is in 2 folds. The first one labelled as HW1 and the second labelled as HW2. In HW1 I analysed a wine dataset using a model in python. I also predicted and evaluated the model's precison and accuracy. Finally I used python to create a decison tree and a confusion matrix. In HW2 I created a model in python, trained the model, analysed the model and set up an enironment to visualize my image using yolov5.
# Table Content
  * Technologies Used
  * Installation
  * Usage
  * Project Structures
  * Examples
  * Assignment Requirements
  * Contributing
  * License
  * Contact
# Technologies Used
* Language: Python 3.9+
* Libraries: 
- [ ] Graphviz: For data visualization
- [ ] Pydot: For visualizing data
- [ ] Pytorch: For machine learning libraries
- [ ] Pandas: For data manipulation
- [ ] CV2: For openCV library
- [ ] Matplotlib: For data visualization
- [ ] Seaborn: For statistical graphs
- [ ] Scikit-learn (sklearn): For machine learning
- [ ] NumPy: For numerical computations
# HW1
1. Load Dataset and Visualize Scatter Plot:
```# Load the Wine Quality dataset
wine = datasets.load_wine()
X = wine.data  # Features
Y = wine.target  # Target variable (wine quality)

# Create a DataFrame for better visualization
wine_df = pd.DataFrame(X, columns=wine.feature_names)
wine_df['target'] = Y

# Display the feature names
print("Feature names:", wine.feature_names)
# Display the first few rows of the dataset
wine_df.head()
# Visualize the data
plt.figure(figsize=(10, 6))
plt.scatter(wine_df['alcohol'], wine_df['malic_acid'], c=wine_df['target'], cmap='coolwarm', s=30)

plt.title(f"Wine Quality Dataset")
plt.xlabel('alcohol') 
plt.ylabel('malic_acid')
plt.colorbar(ticks=np.unique(Y), label='Quality')
plt.show()

# Standardize features
scaler = StandardScaler()
X2 = scaler.fit_transform(X)

# Split the data

X_train, X_test, Y_train, Y_test = train_test_split(X, Y, test_size=0.3, random_state=42)

# Train SVM
svm = SVC(kernel='linear')
svm.fit(X_train, Y_train)  

Y_pred = svm.predict(X_test)

# Make predictions and calculate accuracy
accuracy = accuracy_score(Y_test , Y_pred)
print(f"Accuracy of the SVM model: {accuracy:.2f}")
```
# Results
 

# Assignment Requirements
### Completed Requirements

* [x] Requirement 1: Decision tree
* [x] Requirement 2: Logistic Regression
* [x] Requirement 3: Prediction and Evaluation
* [x] Requirement 4: Yolov5
* [x] Requirement 5: Building Models

# Known Issues
* Issue 1: One of the primary challenges encountered is ensuring that all models are well-defined before execution. Ambiguities in model structure, parameters, or variable definitions can lead to inconsistent outputs or execution errors. To mitigate this, it is essential to: Clearly define all input parameters, boundary conditions, and model variables prior to simulation. Verify consistency between theoretical assumptions and the implemented code. Maintain organized documentation outlining each model’s purpose, scope, and dependencies. This ensures that the simulation or computation reflects the intended design and minimizes debugging complexity later in the workflow.
* Issue 2: Another common issue involves library dependencies that must be executed in sequence or initialized at the top of the script for the code to function correctly. Some libraries load critical configurations or global variables that downstream functions rely on.
# Future Improvements
 * Error handling lacks sufficient diagnostic detail, making debugging unnecessarily time-consuming. Enhancing error message specificity and integrating contextual suggestions will improve user experience and accelerate issue resolution.
 * The system currently executes tasks sequentially, resulting in slower performance during complex or high-volume computations. Implementing parallel or distributed processing will enhance computational efficiency and reduce runtime for large datasets.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

# Acknowledgments
* Course: NANO 706 - System and Computational BIOL
* Instructor: Dr. Sam Oliviera PhD 
* Institution: North Carolina A & T University
* Semester: Fall 2025
# Contact
Your Name

Email: ddavis10@aggies.ncat.edu
GitHub: https://github.com/ddavis10-sudo

Note: This project was created as part of an academic assignment. Please refer to your institution's academic integrity policy before using this code.
