# Book Recommendation Engine (KNN)

This a book recommendation algorithm that was built using K-Nearest Neighbors (KNN) algorithm. The model recommends similar books based on user rating patterns using the Book-Crossing dataset. The goal here was to implement a function ```get_recommends(book_title)``` that returns a list of 5 recommended books similar to the input title, based on collaborative filtering.

## My Contribution
- Filtered the uploaded data:
  - Removed users with fewer than 200 ratings
  - Removed books with fewer than 100 ratings
- Created a **pivot table** to transform the data into a user-book matrix
- Converted the matrix to a sparse formal using **csr_matrix** for efficiency
- Trained a NearestNeighbors model using cosine similarity
- Implmeneted the ```get_recommends()``` function to return similar books and their distances
- Tested the system using a sample book title to validate the model's recommendations

## Strategy Summary
The recommended system is based on the standard collaborative filtering, where books are considered similar if they are rated similarly by many users. The key steps in building this included:
- Dimensionality reduction through filtering to ensure meaningful statistics
- Cosine distance metric to evaluate book similarity in high-dimensional space
- Use of KNN to identify the closest book vectors based on used interaction patterns

## Key skills developed
- Gained experiences with collaborative filtering and real-world recommendation systems
- Learned to manipulate large datasets using Pandas and NumPy
- Built and evaluated a working recommendation engine using scikit-learn
- Applied dimensionality reduction techniques to ensure model accuracy and speed
