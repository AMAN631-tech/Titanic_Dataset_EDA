
# Titanic Dataset Analysis & Preprocessing
This project explores and preprocesses the famous Titanic dataset to prepare it for machine learning tasks. It includes handling missing data, encoding categorical variables, feature engineering, and data visualization.

 Dataset Description
The Titanic dataset includes passenger details such as:

Name, Sex, Age

Ticket, Fare, Cabin

Embarked (Port of Embarkation)

Pclass (Passenger Class)

SibSp (siblings/spouses aboard)

Parch (parents/children aboard)

Survived (Target variable: 0 = No, 1 = Yes)

 Tasks Performed
 
🔹 **1. Data Cleaning**
Checked and handled missing values in key columns (Age, Embarked, Cabin).

Dropped or filled nulls appropriately.

🔹 **2. Feature Engineering**
Extracted Title from the Name column using regex (Mr, Mrs, Miss, etc.).

Grouped rare titles into broader categories (Royal, Officer).

Converted Title into numeric format using One-Hot Encoding and Target Guided Encoding.

🔹 **3. Encoding Categorical Variables**
Applied One-Hot Encoding to:

Embarked → Converted to binary columns (S, C, Q).

Title → Expanded into multiple binary columns.

Used pd.get_dummies() with and without prefix for clean column naming.

Also demonstrated encoding using sklearn.preprocessing.OneHotEncoder.

🔹 **4. Data Visualization**
Created a correlation heatmap to analyze relationships between features.

Used seaborn heatmap with:

annot=True for value labels

Custom colormaps like 'coolwarm', 'viridis', etc.

square=True for balanced cell shape

Font size adjustments for readability

🔹 **5. Column Management**
Dropped original columns like Title and Embarked after encoding to avoid redundancy.

 **Libraries Used**
Python (Pandas, NumPy)

Matplotlib, Seaborn for visualization

Scikit-learn for preprocessing and encoding

