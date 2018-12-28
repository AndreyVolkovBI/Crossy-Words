# Crossy words: word matrix
Library that generates the word matrix in a way to have multiple words in one 5x5 matrix.
## Available methods:
`**getMatrix(lang=”en”)**` – returns two values: a list of lists representing a 5x5 matrix and a dictionary of coordinates of a specific word {word: [coordinates in matrix]}

lang - "en", "ru"

`**printMatrix(matrix)**` - prints generated matrix

`**printWords(matrix)**` - prints generated words with coordinates of letters in the matrix

```python
import crossy-words as cw

matrix, words = cw.getMatrix("en")  # getting a matrix and words in it

cw.printMatrix(matrix)  # printing matrix
print()
cw.printWords(words)  # printing words in it
```
Output:
```
t a t s o
r h l k b
s o w k t
g a n h n
e t h i a

think - [[4, 1], [4, 2], [4, 3], [3, 4], [2, 3]]
thank - [[2, 4], [3, 3], [4, 4], [3, 4], [2, 3]]
own - [[2, 1], [2, 2], [3, 2]]
show - [[2, 0], [1, 1], [2, 1], [2, 2]]
talk - [[0, 2], [0, 1], [1, 2], [1, 3]]
start - [[0, 3], [0, 2], [0, 1], [1, 0], [0, 0]]

```
