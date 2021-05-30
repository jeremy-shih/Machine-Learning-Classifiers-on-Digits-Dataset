AUTHOR: JEREMY SHIH

OVERVIEW: Applied various machine learning classification algorithms including Naive Bayes, Parzen Window, Radial Basis Function Neural Network, and Support Vector Machine on 'trainFeatures42k.xls' data.

DATA USED: The data used ('trainFeatures42k.xls') is transformed from a 'train.csv' file that contains gray-scale images of hand-drawn digits, from 0 to 9 was used. Each image is 28 pixels in height and 28 pixels in width for a total of 784 pixels. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel (high numbers meaning darker, between 0 and 255). The first column is the "label" of the digit, the rest of the columns contain the pixel-values of the associated image. The 2-dimensional Discrete Cosine Transform of each matrix is taken, and the vertical, horizontal and diagonal coefficients from the transform is extracted. The 'trainFeatures42k.xls' file contains 42,000 observations and 60 features, 20 from each direction (vertical, horizontal, diagonal).

DATA PIPELINE: reading in the data, applying Fisher multi class feature ranking, normalization techniques, outlier removal and 5-fold cross validation

CONCLUSION: The results showed that the combination of Normalization of Type 4 (normalization of the data between a and b, where a = -1 and b = 1), followed by Wilk’s Outlier Removal and a Support Vector Machine Classifier gave the highest classification accuracy.
