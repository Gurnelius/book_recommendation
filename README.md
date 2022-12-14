
# Book Recommendation using K-Nearest Neighbors

In this challenge, we create a book recommendation algorithm using K-Nearest Neighbors.

## About the dataset
The project uses the Book-Crossings dataset. This dataset contains 1.1 million ratings (scale of 1-10) of 270,000 books by 90,000 users.

# Summary
After importing and cleaning the data, we use NearestNeighbors from sklearn.neighbors to develop a model that shows books that are similar to a given book. The Nearest Neighbors algorithm measures the distance to determine the “closeness” of instances.

The function get_recommends takes a book title (from the dataset) as an argument and returns a list of 5 similar books with their distances from the book argument.

This code:

```get_recommends("The Queen of the Damned (Vampire Chronicles (Paperback))")```

Returns:

```
[
  'The Queen of the Damned (Vampire Chronicles (Paperback))',
  [
    ['Catch 22', 0.793983519077301], 
    ['The Witching Hour (Lives of the Mayfair Witches)', 0.7448656558990479], 
    ['Interview with the Vampire', 0.7345068454742432],
    ['The Tale of the Body Thief (Vampire Chronicles (Paperback))', 0.5376338362693787],
    ['The Vampire Lestat (Vampire Chronicles, Book II)', 0.5178412199020386]
  ]
]
```

The first element in the list is the book title passed into the function. 
The second element in the list is a list of five more lists.
Each of the five lists contains a recommended book and the distance
from the recommended book to the book passed into the function.

This project is part of  Machine Learning Certification by 
[freeCodeCamp](https://www.freecodecamp.org/learn/machine-learning-with-python). 