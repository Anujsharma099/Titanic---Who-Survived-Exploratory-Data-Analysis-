🚢 Titanic: Survival Prediction Analysis
📌 Project Overview
This project performs a comprehensive Exploratory Data Analysis (EDA) on the Titanic passenger manifest. The goal is to move beyond simple statistics and uncover the underlying social and physical factors—such as socio-economic status, gender, and age—that determined a passenger's chance of survival.

🛠️ Key Skills & Tools
Language: Python

Libraries:

Pandas & NumPy: For data cleaning and structural manipulation.

Matplotlib & Seaborn: For multivariate data visualization.

Concepts: Data Imputation, Feature Engineering, Categorical Encoding, and Statistical Analysis.

📊 Key Insights & Analytical Steps
1. Advanced Data Cleaning
Handling Sparsity: Identified that the Cabin column was missing over 70% of its data; logically dropped the feature to prevent model noise.

Strategic Imputation: * Filled missing Age values using the Median to avoid the influence of outliers.

Filled Embarked missing values using the Mode (most frequent port).

2. Feature Engineering (Creating Value)
Instead of relying only on raw columns, I engineered new features to find hidden patterns:

Family Dynamics: Combined SibSp (siblings/spouses) and Parch (parents/children) to calculate FamilySize.

Independence Factor: Created an IsAlone binary feature to test the hypothesis that passengers traveling alone had different survival rates than those in groups.

3. Critical Findings
The Gender Gap: Confirmed the "Women and Children First" protocol, with female passengers showing a survival rate significantly higher than males.

Class Disparity: Discovered a clear correlation between Pclass and survival, showing that socio-economic status was a physical barrier to safety resources.

Age Trends: Used distribution plots to show that infants and young children had a higher probability of survival, while the elderly were more vulnerable.

🚀 How to Use
Clone the repository:

Bash
git clone https://github.com/YourUsername/Titanic-Analysis.git
Install dependencies:

Bash
pip install pandas numpy seaborn matplotlib
Run the Analysis: Open eda_1_.ipynb in Jupyter Notebook or Google Colab.

📁 Project Structure
eda_1_.ipynb: The complete analytical workflow and visualizations.

train.csv: The passenger dataset used for training and exploration.
