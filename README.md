
<h3 align="center">VGG16 Convolutional Neural Net Object Detection</h3>

  <p align="center">
    <br/>
    <a href="https://github.com/charlelotfalla/VGG16-CNN-Object-Detection"><strong>Explore the docs »</strong></a>
  </p>
</p>

<br />

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#data">Data</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    <li>
      <a href="#Usage">Usage</a>
      <ul>
      </ul>
    </li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

The purpose of the project is to analyze the research findings trends in an extensive list of medical publications (Abstracts, Full-Text). The data is extracted from PubMed.com in form of a csv. Then the data is cleaned, lemmatized, stemmed and then used to create a dictionary of either single phrases or multi-phrases. Then the topic model is designed using Latent Dirichlet Allocation. LDA allows each document (abstract) to be described by a distribution of topics and each topic is described by a distribution of words. 

The number of topics, hyperparameter k, in the model is optimized using a gridsearch function with the scoring metric called 'Coherence Score'. Coherence score measures the degree of semantic similarity between high scoring words in each of the topics.

The k with the highest coherence score is used to build the final model. The LDA model is used on the dataset to create the Document-topic & topic-word probability distributions. 

Then LDAVis library is used to create a dashboard for topic visualizations.


### Data

Source: [The CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz) <br />
Copyright: Open-source <br />
Variables:10000x3072 array of uint8s. Each row of the array stores a 32x32 colour image. The first 1024 entries contain the red channel values, the next 1024 the green, and the final 1024 the blue. The image is stored in row-major order, so that the first 32 entries of the array are the red channel values of the first row of the image. <br />


<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple steps.


### Prerequisites

Any python IDE or Code Editor (Spyder, Jupyter Notebook, Sublime text 3, ... etc).


### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/charlelotfalla/COVID-19-Publications-Topic-Model.git
   ```
2. Install Python packages
   ```sh
   pip install nbimporter lemmatizer ldamodel gensim pyLDAvis re nltk spacy pickle os scispacy random string
   ```
   
<br />

<!-- USAGE -->
## Usage

This project can be used for any type of topic modeling in big sets of documents (publications, articles, news, etc...). It's useful the most in the medical field as the stemmer and lemmatizer used are more specific to medical data. A solution to this is replacing the medical-specific stemmar, SciSpacy, with a more general version, from NLTK. 

<br />

<!-- CONTACT -->
## Contact

Charle Lotfalla - [@charle_lotfalla](https://twitter.com/charle_lotfalla) - charlelotfalla@gmail.com





  


  
