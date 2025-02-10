# Mushroom_edibility_classification

**Overview**

This project aims to classify mushrooms as edible or poisonous using machine learning techniques. The dataset contains various features such as cap shape, gill color, stem height, and more, which help in determining the edibility of mushrooms.

**Dataset**
The dataset consists of multiple categorical and numerical features describing different properties of mushrooms. Some key attributes include:
cap-diameter: Size of the mushroom cap.
cap-shape: Shape of the cap.
gill-attachment: The way gills are attached to the stem.
gill-color: Color of the gills.
stem-height: Height of the stem.
stem-width: Width of the stem.
stem-color: Color of the stem.
season: Season in which the mushroom grows.
class: Label indicating whether the mushroom is edible (0) or poisonous (1).

Methodology

1. Data Preprocessing

Handled missing values.

Encoded categorical features using Label Encoding / One-Hot Encoding.

Standardized numerical features using Z-score normalization.

2. Outlier Detection & Removal

Calculated Z-scores for numerical columns.

Removed rows where |Z-score| > 3.

3. Model Training & Evaluation

Used K-Nearest Neighbors (k-NN) for classification.

Evaluated model performance using:

Error Rate for different values of k.

Accuracy, Precision, Recall, and F1-score.

Installation & Setup

Clone the repository:

git clone https://github.com/your-username/mushroom-classification.git
cd mushroom-classification

Create and activate a virtual environment:

python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

Install dependencies:

pip install -r requirements.txt

Run the classification script:

python classify_mushrooms.py

GitHub Usage

Creating a New Branch

Before making changes, create a new branch:

  git checkout -b feature-branch

Committing Changes

After making changes, commit them:

  git add .
  git commit -m "Added new feature"

Pushing Changes

Push the changes to GitHub:

  git push origin feature-branch

Creating a Pull Request (PR)

Go to the repository on GitHub.

Click on Pull Requests > New Pull Request.

Select your branch and compare it with the main branch.

Write a description and submit the PR for review.

Results & Findings

The best k-value was determined by analyzing the Error Rate vs. k-value plot.

The final model achieved high accuracy, successfully distinguishing edible and poisonous mushrooms.

Removing outliers improved model performance by reducing noise in the data.

Future Improvements

Experiment with other models like Random Forest, SVM, and Neural Networks.

Implement feature selection techniques to improve efficiency.

Deploy the model as a web application for real-time classification.

Contributing

If you would like to contribute, feel free to fork the repository, create a new branch, and submit a pull request!

License

This project is licensed under the MIT License.

