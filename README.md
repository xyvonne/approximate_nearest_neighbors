## About

This is a lab we made at EPITA School, concerning Approximate Algorithms
and Data Structures, and more specifically Nearest Neighbors search.

It is written in Python 3.

The dataset is the training part of 20newsgroups, which consists in
11,314 documents spread in 20 topics.

First, we make a dimension reduction (dim=128) by performing a LSA (Latent
Semantic Analysis) on the TF-IDF matrix.
Then, we make a random sample of 20 documents (one per topic).
For each document in this sample, represented as a 128-dimensional vector
(after TF-IDF + LSA), we compute and return its 8 nearest neighbors,
using either:
- cosine similarity (this can be considered as our reference);
- Product Quantization and Euclidean distance (this is our approximation).

A more detailed version of the assignment (in French), along with the full
description of our implementation (in English), are to be found in the notebook.

## Execution

Run the `approx_nn.ipynb` file as a Jupyter Notebook, and run all cells in it.

## Dependencies

* Everything required for a Jupyter Notebook to run.
* numpy, scikit-learn

## References

* 20newsgroups: http://qwone.com/~jason/20Newsgroups/
* Product Quantization:
https://lear.inrialpes.fr/pubs/2011/JDS11/jegou_searching_with_quantization.pdf
http://mccormickml.com/2017/10/13/product-quantizer-tutorial-part-1/

## Author

Xavier YVONNE: xavier.yvonne@epita.fr
