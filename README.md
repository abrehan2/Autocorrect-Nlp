# Auto-Correct and String Manipulation

This repository contains Python code for text preprocessing and manipulation, including auto-correction functionalities using dynamic programming inspired by minimum edit distance. The implemented tasks are outlined as follows:

---

## Part 1: Data Preprocessing

### Task 1.1: `process_data` function
- Reads a corpus (text file).
- Converts the corpus to lowercase.
- Returns a list of words.

### Task 1.2: `get_count` function
- Returns a dictionary where keys are words, and values are their frequency in the corpus.

### Task 1.3: Computing Word Probabilities
- Calculates the probability of each word appearing when randomly selected from the corpus using the formula: P(wi) = C(wi) / M, where C(wi) is the count of word wi and M is the total number of words.

---

## Part 2: String Manipulations

- `delete_letter` function: Returns all possible strings with one character removed from a given word.
- `replace_letter` function: Returns all possible strings with one character replaced by another different letter.
- `insert_letter` function: Returns all possible strings with an additional character inserted into a given word.

---

## Part 3: Combining the Edits

- `edit_one_letter` function: Generates all possible edits one edit away from a word using delete, replace, and insert operations.
- `edit_two_letters` function: Generates a set of words that are two edits away from a given word using combinations of `edit_one_letter` function.
- `get_corrections` function: Provides spelling suggestions based on minimum edit distance logic, prioritizing words with fewer edits.

---

## Part 4: Minimum Edit Distance

### Dynamic Programming Algorithm
- Computes the minimum number of edits required to convert one string into another.
- Utilizes a table to efficiently calculate edit distances for substrings of source and target strings.

---

### Usage

To effectively use this repository:

1. **Clone the Repository:**
 ```sh
git clone https://github.com/abrehan2/Autocorrect-Nlp.git
```
