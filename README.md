
<h3 align="center">VGGNET Convolutional Neural Net (CNN) Object Detection</h3>

  <p align="center">
    <br/>
    <a href="https://github.com/charlelotfalla/VGGNET-Convolutional-Neural-Network-(CNN)-Object-Detection"><strong>Explore the docs »</strong></a>
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
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

The purpose of the project is build an object detection classifier using CNN architecture. The CIFAR-10 Dataset contains 10 different object classes. 2 classes (deer & dogs) were picked for analysis. Initially, exploratory data analysis on the pixel data for the two classes showed differences in mean and standard deviations of colors for the two classes. Pixels for deer images had less standard deviation than these of dogs. This is explained by the various dog breeds compared to those of deer. 

A base CNN model of 1 convolutional and 1 max pooling layer was built to test on the dataset. The model achieved object detection accuracy of around 85%.

To optimize the model, a VGGNET architecture was used of total 6 convolutional layers & 3 max pooling layers. L1 & L2 regularizations and 3 dropout layers were used to prevent overfitting. The final model achieved 92% val accuracy and 90.5% test accuracy. 


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
   git clone https://github.com/charlelotfalla/VGGNET-Convolutional-Neural-Network-CNN-Object-Detection.git
   ```
2. Install Python packages
   ```sh
   pip install sklearn keras seaborn random 
   ```


<!-- CONTACT -->
## Contact

Twitter: [@charle_lotfalla](https://twitter.com/charle_lotfalla)  

Email: charlelotfalla@gmail.com





  


  
