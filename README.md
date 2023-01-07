# Collaborative filtering with matrix factorization
Collaborative filtering with matrix factorization using Scipy library

## Matrix Factorization for Recommendation Systems
This code contains an implementation of a matrix factorization technique for recommendation systems. It takes as input an interaction matrix containing information about user-item interactions, and returns a list of recommended items for a given user. For the the the movielens 100k was used (https://www.kaggle.com/datasets/prajitdatta/movielens-100k-dataset).

## Requirements
- NumPy
- SciPy
- Pandas

### Usage
To use this code, follow these steps:

Place the csv file containing the ratings in the same directory as the code.
Modify the value of the user_id variable to specify the user for which recommendations are desired.
Run the code.

Output
The code will output a list of recommended items for the specified user, sorted by their predicted ratings.

## Notes
The code normalizes the interaction matrix by subtracting the mean rating for each user and dividing by the standard deviation of the ratings for each user.
The code computes the singular value decomposition (SVD) of the interaction matrix. The number of latent factors used in the SVD can be modified by changing the value of the k parameter in the call to svds.
The code uses the dot product of the matrices obtained from SVD to compute predicted ratings for all items and recommends the highest-rated items to the user.

In the end i compared the results from the naive approach that i used here: https://github.com/Ishikawa7/Simple-Collaborative-Filtering-with-Pandas
