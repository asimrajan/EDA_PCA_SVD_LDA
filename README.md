# EDA, PCA, SVD, LDA HandsOn

## Peformed Exploratory Data Analysis(EDA) on Diabetes.csv

* Loading data, determing attributes & its type and its geometry.
* Generating Summary Statistics
    - Range and Variance of attributes
    - Exploring different Categorical attributes
    - Overview of how data is distributed for each attributes
* Understanding the (in)dependencies among attributes using Covariance Matrix
    - Which pairs co vary
    - Which attributes have high/low corrlation
    - What to infer
* Dimentionality Reduction
    - Feature Selection (Domain Knowledge and depending on correlation between attributes)
    - Principal Component Analysis (PCA)

## Implemented Principal Component Analysis (PCA)

* Principal component are the ordered set of directions/dimensions that captures the most variance with minimum Sum of Squared Error(SSE)
* Is a linear transformation(rotation) of data.
* The line that maximises the SSE, will always maximise the projected variance(i.e will capture the max variance of the data)
* Works only when the data is Ellipsoidal
* Fails when the data is circular in shape. Here Kernel PCA is preferred.

## Implementing Singular-Value Decomposition (SCV)

* A  --> U.S.V
    - A = Original Data Matrix (n x d)
    - U = Eigenvectors along the "Data Points" (n x n)
    - S = (n x d)
    - V = Eigenvectors along the "Dimensions (attributes)" (d x d)

## Implementing Linear Discriminant Analysis (LDA)

* To find the direction that separates the class
* Considers the class label while finding the principal axis UNLIKE PCA
* Objective:
    - Maximise the distance of projected mean of each class (Separate the classes)
    - Minimise the sum of projected variance of each class (Minimise the Overlap between the classes)
* Fails when the classes are inscribed within each other. Here other classifiers are preferred.
