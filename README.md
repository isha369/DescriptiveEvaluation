# Descriptive Evaluation


This repository contains all the code used while developing the descriptive answer evaluator at [Ramaiah Institute of Technology](http://www.msrit.edu/index.html). Done as a part of the project 'Lightweight Container-based Framework in Cloud Environment for Automated Online Assessment for Computer Science Courses' funded by VGST, Govt of Karnataka

## Contributors
- [Isha Gupta](https://github.com/isha369)
- [Mrigank Khandelwal](https://github.com/Mrigankkh)
- [Sreya Salil](https://github.com/SreyaSalil)

## About Each Project
### BERT + Cosine Similarity
___________________________________

Uses BERT and Cosine Similairty to find the semantic similarity between two sentences

### GloVe
___________________________________

Uses GloVe embeddings and Manhattan LSTM to determine semantic similarity between the answer key and student answers.
#### Files Required
- [train_main.csv](https://drive.google.com/file/d/1Mh3sUDOSNa6g6tqhZD1eoqCZlBXkLErw/view?usp=sharing)
- [GloVe Embeddings](https://drive.google.com/file/d/1epXvS0xWlTy9tmcW1LM2HtngogwcuFTf/view?usp=sharing)

### Hewlett Dataset
_________________________
Uses GloVe, Poincaré and Word2Vec embeddings along with Manhattan LSTM to find semantic similairty between short answers from the Hewlett Dataset
#### Additional Files Required:
- [GloVe Embeddings](https://drive.google.com/file/d/1epXvS0xWlTy9tmcW1LM2HtngogwcuFTf/view?usp=sharing)
- [Word2Vec Embeddings](https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/view?usp=sharing&resourcekey=0-wjGZdNAUop6WykTtMip30g)
- [Hewlett Dataset](https://drive.google.com/file/d/1UW1SOGspJ3Vhs-vKQ2Ey6xGiFZvzB4-L/view?usp=sharing)
#### Notes
- The Poincaré embeddings are automatically generated from the dataset in the notebook
- The dataset must be transformed to a certain format before running the codes. Use this [notebook.](https://colab.research.google.com/drive/1lRd7_0itJnbUVoR_EtaJsCpziHGLJ3rb?usp=sharing)

### Extracting Keywords and Keyword Matching
____________________________________________
Takes the OOP dataset and extracts keywords from both the answer key and student answers. Keyword matching techniques are used to check which matching technique accurately finds the similairty between the keywords. The keyword extraction techniques are also evaluated using mean average precision.
#### Datasets used
- [train_main.csv](https://drive.google.com/file/d/1Mh3sUDOSNa6g6tqhZD1eoqCZlBXkLErw/view?usp=sharing)
- [Define OOPs.csv](https://drive.google.com/file/d/1s_A9356nA3Ns11MV1eP8SjnbMb6jo4LT/view?usp=sharing)

### Knowledge Based Measures
______________________________________
Uses Knowledge based measures like Lin, Jiang-Conrath Resnik and WuPalmer to determine semantic similarity between the answer key and student answers.
#### Dataset used
- [train_main.csv](https://drive.google.com/file/d/1Mh3sUDOSNa6g6tqhZD1eoqCZlBXkLErw/view?usp=sharing)

### Poincaré
_______________________________
Uses Poincaré embeddings and Manhattan LSTM to find semantic similairty between the answer key and student answers.
#### Dataset used
- [train_main.csv](https://drive.google.com/file/d/1Mh3sUDOSNa6g6tqhZD1eoqCZlBXkLErw/view?usp=sharing)
#### Notes
- The Poincaré embeddings are automatically generated from the dataset in the notebook

### Semantic Similarity Functions
_______________________________
Uses tf-idf vectors, Pairwise similarity, word2vec embeddings, Doc2vec model and BERT to find semantic similairty between ta list of documents.
#### Files Required
- [Word2Vec Embeddings](https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit?usp=sharing)

### Descriptive Answer Evaluator
_________________________________________________
Uses RAKE keyword Extractor, Keyphrase extracter using TF-IDF and BERT + Cosine similairty to evaluate student answers.
#### Files Required
- [Define OOPs.csv](https://drive.google.com/file/d/1s_A9356nA3Ns11MV1eP8SjnbMb6jo4LT/view?usp=sharing)
- [Word2Vec Embeddings](https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit?usp=sharing)

### Word2Vec
_______________________________
Uses Word2Vec embeddings and Manhattan LSTM to determine semantic similarity between the answer key and student answers.
#### Files Required
- [train_main.csv](https://drive.google.com/file/d/1Mh3sUDOSNa6g6tqhZD1eoqCZlBXkLErw/view?usp=sharing)
- [Word2Vec Embeddings](https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit?usp=sharing)

### fastText
__________________________________
Uses fastText embeddings and Manhattan LSTM to determine semantic similarity between the answer key and student answers.
#### Dataset used
- [train_main.csv](https://drive.google.com/file/d/1Mh3sUDOSNa6g6tqhZD1eoqCZlBXkLErw/view?usp=sharing)
#### Notes
- The fastText embeddings are downloaded from GitHub in the notebook

### Node2Vec
____________________________
Generates a graph from the corpus of answers. Then generates embeddings by performing a random walk on the graph. These embeddings with Manhattan LSTM are used to determine semantic similarity between the answer key and student answers.
#### Dataset used
- [train_main.csv](https://drive.google.com/file/d/1Mh3sUDOSNa6g6tqhZD1eoqCZlBXkLErw/view?usp=sharing)
