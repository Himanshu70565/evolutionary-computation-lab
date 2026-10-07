# Question 4: Image Classification

This folder contains the genetic-programming image-classification
implementation for the FEI 1 and FEI 2 datasets.

## Classification File

The main classification program is:

- [`src/IDGP_main.py`](src/IDGP_main.py)

## Pattern Files

The generated pattern files contain the feature vectors extracted from the
images together with their class labels. Each dataset has separate training
and testing files:

### FEI 1

- [`data/f1/f1_train_patterns.csv`](data/f1/f1_train_patterns.csv)
- [`data/f1/f1_test_patterns.csv`](data/f1/f1_test_patterns.csv)

### FEI 2

- [`data/f2/f2_train_patterns.csv`](data/f2/f2_train_patterns.csv)
- [`data/f2/f2_test_patterns.csv`](data/f2/f2_test_patterns.csv)

The training pattern files are used to train the classifier using classification_4.2, while the testing
pattern files contain unseen examples for evaluating classification
performance.

## Required Packages

Install the required Python packages with:

```bash
pip install deap numpy pandas scipy scikit-image scikit-learn pillow
```
