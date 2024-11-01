# Classifier Performance Evaluation on Loan Applications

## Project Overview

This project aims to design and evaluate several well-known binary classifiers using real-world data collected from loan applications. The classifiers implemented include:

- Decision Tree
- k-Nearest Neighbors (kNN)
- Linear Discriminant Analysis (LDA)
- Support Vector Machine (SVM)

Additionally, the project explores how dimensionality reduction achieved via Principal Component Analysis (PCA) affects the performance of some of these classifiers.

## Dataset

The data for this project is provided in two separate files:

- `TrainingData.csv`: Contains 900 samples (450 approved and 450 denied applications) with 27 features (e.g., Age, Annual Income) and a label (LoanApproved in the last column).
- `TestingData.csv`: Contains 400 samples (200 approved and 200 denied applications) for evaluating classifier performance.

## Project Structure
/Suryodaya's_Classifier_Performance_Evaluation_on_Loan_Applications_
│
├── TrainingData.csv
├── TestingData.csv
├── Classifier_Performance_Evaluation.ipynb
└── README.md

## Installation

To run this project, you need to have Python installed along with the following libraries:

- pandas
- numpy
- matplotlib
- scikit-learn
- google.colab (if using Google Colab)

You can install the required libraries using pip:

## Usage

1. Clone the repository or download the project files.
2. Open the Jupyter Notebook `Classifier_Performance_Evaluation.ipynb`.
3. Run the notebook cells sequentially to train the classifiers and evaluate their performance.

## Classifier Implementation

### 1. Linear Discriminant Analysis (LDA)

- LDA is used to find a suitable direction for classification.
- The classifier's performance is evaluated by varying the threshold and calculating Type 1 and Type 2 error rates.

### 2. Decision Tree

- A decision tree classifier is implemented using the CART algorithm.
- The classifier's performance is evaluated using confusion matrices and classification reports.

### 3. k-Nearest Neighbors (kNN)

- The performance of the kNN algorithm is evaluated for different values of k (1, 3, 5, 10).
- Confusion matrices and error rates are calculated for each k value.

### 4. Support Vector Machine (SVM)

- An SVM classifier with a soft margin is implemented.
- The classifier's performance is evaluated using confusion matrices and classification reports.

## Dimensionality Reduction with PCA

- PCA is applied to reduce the dimensionality of the dataset.
- The kNN and SVM classifiers are retrained using PCA-transformed features, and their performance is compared to the original classifiers.

## Results

- The results of each classifier's performance, including Type 1 and Type 2 error rates, are summarized in the notebook.
- Visualizations such as confusion matrices and error rate plots are included to aid in understanding the classifier performance.

## Conclusion

- The project concludes with a comparison of the classifiers' performances and insights into the impact of PCA on classification accuracy.
- Future work may include further hyperparameter tuning and exploring additional classifiers.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Scikit-learn Documentation](https://scikit-learn.org/stable/documentation.html)
- [Pandas Documentation](https://pandas.pydata.org/pandas-docs/stable/)
- [Matplotlib Documentation](https://matplotlib.org/stable/contents.html)
