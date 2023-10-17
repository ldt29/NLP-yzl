    # Natural Language Processing

## 9.19 lecture 1

### Intro
- What NLP
- Why NLP
- Where NLP

### Sub-languages

- Heterogeneity of language
- Unigram Type-Token Curve 
- Zipf’s Law

### Probabilistic view of natural language
- Surface Forms and Hidden Forms
- Source Channel Paradigm
- ASR
- Topic Detection



### Word vectors


- Representing Words By Their Context

- Linear Transformation of One-Hot Vectors

## 9.26 lecture 2

### Distributional and Distributed Representations

- Coarse Coding
- how to create
    - use logical assocaition
    - feature learning

- everything can be vectorized

###  Word2vec Embedding

- Objective Function

- Prediction Fucntion
    - sofemax
- how many vectors GD 
    |V|+1
- Skip-Gram Model with Negative Sampling

### Count-based Word Embedding

- Windows v.s. full document
    - Dimensionality Reduction SVD

- Count-Based v.s. Direct Prediction

### Glove Embedding

- ratio

### Evaluation of word embeddings

- intrinic

- extrinic


## 10.10 lecture 3

### Unigram estimation

* Estimating Probabilities of Words
  * N-gram 
    * unseen words
    * infrequent words
    * Dealing With Unseen Words: <UNK>

* Good-Turing estimation v.s. MLE   
  * Frequency of Frequencies
  * regression to the mean

* Dirchlet smoothing  
  * Dirichlet Prior

### Language Modeling
* Ngram models
    * Storage Problem with N-Gram Models
* smoothing
  * Linear Interpolation
  * Absolute Discounting
  * Kneser-Ney (KN) Smoothing
  


## 10.17 lecture 4
### Neural language models
* A Fixed-Window Neural Language Model

### RNN language models
* Core idea: apply the same weights W repeatedly
* Shift invariance, a very strong inductive bias!
* Training an RNN Language Model
* Backpropagation for RNNs
  * backpropagation through time
  * For efficient implementation, losses at different timesteps are backpropagated at the same time.
* Construct Mini-Batches for LM
  * Sentence-Level Batching
  * Fixed-Length Batching
  * Continuous Batching
  * Shuffled Batching
  * Vanishing Gradients
  * Long-Distance Dependencies in Language  
  * Exploding Gradients

### LSTM language models
* Long Short-Term Memory (LSTM) Networks
* Key idea: make additive connections and gating between timesteps
  
### LM Evaluation
* Intrisic Evaluation of Language Models
  * Perplexity
* Extrinsic Evaluation of LMs
  * Evaluating LMs on Speech Recognition

### Usage of RNNs

### Improved architectures of RNNs
