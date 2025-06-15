# AI_lab
import seaborn as sns
import matplotlib.pyplot as plt

# For target variable
sns.histplot(y, kde=True)
plt.title("Distribution of Target Variable")
plt.show()

# For a few features
for col in X.select_dtypes(include='number').columns[:3]:  # first 3 numerical features
    sns.histplot(X[col], kde=True)
    plt.title(f"Distribution of {col}")
    plt.show()
